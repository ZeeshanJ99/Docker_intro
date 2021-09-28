# Docker

<img src = "https://user-images.githubusercontent.com/88186084/134984570-9b5ef641-e3dd-4d30-8a1d-b134831d923b.gif">

----------------------------------------

## What is Docker

A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. A Docker container image is a lightweight, standalone, 
executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.

Docker images contain all the dependencies needed to execute code inside a container, so containers that move between Docker environments with the same OS work with no changes. 
Docker uses resource isolation in the OS kernel to run multiple containers on the same OS.

Docker is a set of platform as a service products that use OS-level virtualization to deliver software in packages called containers. 
Containers are isolated from one another and bundle their own software, libraries and configuration files; they can communicate with each other through well-defined channels

![image](https://user-images.githubusercontent.com/88186084/134954424-68fb10c9-eaa6-4c30-999d-f8073104a51b.png)

--------------------------------------------------

## Docker Architecture

![image](https://user-images.githubusercontent.com/88186084/134984555-779db2f3-8533-4818-ba53-8209d459588b.png)>

-------------------------------------------

## Benefits of Docker

### Consistent and Isolated Environment
- Using containers developers can create predictable environments that are isolated from other apps.

### Cost-effectiveness with Fast Deployment
- Docker-powered containers are known for decreasing deployment time to seconds. Traditionally, things like provisioning, getting the hardware up and running would take ages. When each process is put into a container, it can be shared with new apps. The process of deployment becomes swift.

### Mobility – Ability to Run Anywhere
- Docker images are free of environmental limitations, and that makes any deployment consistent, movable (portable), and scalable. Containers have the added benefit of running anywhere, providing it is targeted at the OS (Win, Mac OS, Linux, VMs, On-prem, in Public Cloud), which is a huge advantage for both development and deployment. The widespread popularity of the Docker image format for containers further helps. It has been adopted by leading cloud providers, including Amazon Web Services (AWS) and Microsoft Azure. In addition, you have powerful orchestration systems such as Kubernetes, and products such as AWS ECS or Azure Container Instances are mighty useful in terms of mobility.

### Repeatability and Automation
- You are building code with repeatable infrastructure and config. This speeds up the development process tremendously. It must be pointed out that Docker images are often small. Consequently, you get fast delivery and, again, shorter deployment for new application containers.

### Test, Roll Back and Deploy
- Docker images are easily versioned, which makes them easy to roll back if you need to do so. If there is a problem with the current iteration of the image, just roll back to the older version. The whole process means you are creating the perfect environment for continuous integration and continuous deployment (CI/CD). Docker containers are set to retain all configs and dependencies internally. Now, you have a fast and easy way of checking for discrepancies.

### Flexibility
- If you need to perform an upgrade during a product’s release cycle, you can easily make the necessary changes to Docker containers, test them, and roll out new containers. This sort of flexibility is another key advantage of using Docker. Docker really allows you to build, test, and release images that can be deployed across multiple servers. Even if a new security patch is available, the process remains the same. Additionally, Docker allows you to start and stop services, or apps rapidly, which is especially useful within the cloud environment.

### Collaboration, Modularity and Scaling
- The Docker method of containerization allows you to segment an application so you can refresh, clean up, repair without even taking down the entire app. Furthermore, with Docker you can build an architecture for applications comprising of small processes that communicate with each other via APIs. From there, developers share and collaborate, solving any potential issues quickly. At this stage, the development cycle is completed and all issues are resolved, with no massive overhaul needed – this is extremely cost-effective and time-saving.

![image](https://user-images.githubusercontent.com/88186084/134954807-00c0e464-a343-4e19-b16a-3be6bfce7108.png)

-------------------------------------------------

## What are Microservices

Microservice architecture, or simply microservices, is a distinctive method of developing software systems that tries to focus on building single-function modules with well-defined interfaces and operations.

In the simplest form, they help build an application as a suite of small services, each running in its own process and are independently deployable. These services may be written in different programming languages and may use different data storage techniques. While this results in the development of systems that are scalable and flexible, it needs a dynamic makeover. Microservices are often connected via APIs, and can leverage many of the same tools and solutions that have grown in the RESTful and web service ecosystem.

![image](https://user-images.githubusercontent.com/88186084/134953976-e038f3b1-21be-42fc-9d67-b62c8de7b6b8.png)

--------------------------------------------------

## Differences between Microservices and Monolith architecture

Monolithic architecture  is based on a single application. This system comes with various advantages; first, you can develop faster with the essential requirements. It also makes the application quicker since there is no use of APIs.  Maintaining applications becomes problematic if it is not designed well. And this is because processes are likely to be tightly coupled. Also, Monolithic puts all of the functionality into a single process monitoring becomes one hell of a task! So, scalability, availability, and reliability get tough for the same reason.

While a monolithic application is a single unified unit, a microservices architecture breaks it down into a collection of smaller independent units. These units carry out every application process as a separate service. So all the services have their own logic and the database as well as perform the specific functions

![image](https://user-images.githubusercontent.com/88186084/134954176-43a99b4c-d092-4370-a784-46fbd2ec44d9.png)

-----------------------------------------------------

## Differences between VM and Docker

Docker is container based technology and containers are just user space of the operating system. At the low level, a container is just a set of processes that are isolated from the rest of the system, running from a distinct image that provides all files necessary to support the processes. It is built for running applications. In Docker, the containers running share the host OS kernel.

<img src = "https://user-images.githubusercontent.com/88186084/134983025-9d44573c-8d3f-40f6-a363-a1ac605768db.gif">

A Virtual Machine, on the other hand, is not based on container technology. They are made up of user space plus kernel space of an operating system. Under VMs, server hardware is virtualized. Each VM has Operating system (OS) & apps. It shares hardware resource from the host.

![image](https://user-images.githubusercontent.com/88186084/134954577-1966e632-a5c4-404d-a84b-7a621245a2c5.png)

-----------------------------------------------------

# Docker Setup

------------------------------------------

## Step 1 - Where to download

- In order to setup docker first you need to go to https://docs.docker.com/desktop/windows/install/
- On this page ensure that the system requirements of WSL 2 backend are highlighted as such

![image](https://user-images.githubusercontent.com/88186084/134956050-513b9b97-9fe3-4abd-a8dd-f62b8aea7730.png)

--------------------------------------------------------

## Step 2 - Setup wizard

- Once downloaded go through the setup wizard and ensure that the `WSL Windows features` is ticked
- Unpacking files may take some time and you may be required to `restart` your PC at the end of this period

![image](https://user-images.githubusercontent.com/88186084/134958036-ca01537f-fecb-4be8-bfc8-9dfa2323d21e.png)

----------------------------------------------

## Step 3 - Docker ID

- Whilst the files are unpacking we can make our own account on `Docker Hub` 
- Follow this link to the Docker Hub homepage https://hub.docker.com/
- Creating an account is very simple all you have to do is create an `Docker ID` and provide an `email` and `password`
- Once created you will need to verify your email

![image](https://user-images.githubusercontent.com/88186084/134957264-e9bf6c0b-02be-4d62-8c46-99bb2baf5b4d.png)

---------------------------------------------------

## Step 4 - Checking whether Docker is installed

- To check whether Docker has installed correctly open a terminal as admin
- Use the command `docker version` and you should see the following

![image](https://user-images.githubusercontent.com/88186084/134958388-ece53ad1-a3ed-46d4-9d8a-7362943bf8be.png)


------------------------------------------------------------------------

## Step 5 - Docker Desktop

- Once your PC has restarted open the newly installed Docker Desktop
- This may prompt you to download the `WSL kernel update`

![image](https://user-images.githubusercontent.com/88186084/134960239-b016d0ed-4e5e-4080-85fc-c82b74b80688.png)

---------------------------------------------------------------------

## Step 6 - WSL Kernel update

- Follow the link provided https://docs.microsoft.com/en-us/windows/wsl/install-manual
- On `Step 4` you will need to click the link to download the WSL kernel
- Restart your Docker Desktop app

![image](https://user-images.githubusercontent.com/88186084/134959237-90eddaff-bd3c-44cc-94df-b6685036589a.png)


![image](https://user-images.githubusercontent.com/88186084/134958598-450a71c9-2091-4ef9-8e69-ec27b540d821.png)

------------------------------------------------------------------------------

## Step 7 - Configuration

- Make sure you are signed in with the Docker ID we made in `Step 3` of this process
- Go to your Docker settings and ensure that the box to `Enable integration with WSL is ticked`

![image](https://user-images.githubusercontent.com/88186084/134959023-48e004a2-4bdc-474e-a0d9-85742f7c917b.png)

-----------------------------------------------------------------------

## Step 8 - Hello World

The first image we will pull from docker is named `hello-world`. In order to do so these are the commands you should use in a terminal you have ran as admin.

- Use the command `docker pull hello-world` and you should see the following. This will pull this specific image from docker

![image](https://user-images.githubusercontent.com/88186084/134959885-c85b43c2-195c-4b2d-860b-39f106a1ec40.png)

- Using the command `docker images` will show you all the images you have pulled

![image](https://user-images.githubusercontent.com/88186084/134959970-5e22fbaf-641b-4ad1-9d47-9921f0fe12d0.png)

- Using the command `docker run hello-world` will run the specified image. In this case we are running the image named `hello world`

![image](https://user-images.githubusercontent.com/88186084/134960054-c7c7eb0d-6b25-4236-a9de-159ac30bc35e.png)

---------------------------------------------

## Docker Commands
- `docker pull name_of_image` - pulling an image
- `docker run name_of_image` - running an image
- `docker build -t zeeshanj/sre_docker_app:v1` - building an image
-  `docker commit name_of_image:v1` - commit changes
- `docker push name_of_image` - pushing an image to dockerhub repo
- `docker rmi name_of_image:v1 -f` - removing an image

---------------------------------------------------------------

### Lets see an example of an image that is already available on Dockerhub/registry

- Image called `ghost`
- `-d` detatched
- `-p` - the port its run on
- `docker run -d -p 2368:2368 ghost`

- `docker ps` or `docker ps -a` - Checking container state
- go to `localhost:2368` to see the webpage


- stop - start - remove containers
- `docker stop containerid` - stop
- `docker start containerid` - start
- `docker rm e9d6a080b10e` - remove
- Get the `container id` through using `docker ps -a`
- Difference between `stop` and `remove` is that stopped state still holds the same data available whereas remove deletes it completely

--------------------------------------

### Interact with running Container

- Firstly, change the alias `alias docker="winpty docker"`
- Then use this command to shell in `docker exec -it containerid sh`


-------------------------------------------------

## Here are some more docker commands that may be useful:

      attach      Attach local standard input, output, and error streams to a running container
      build       Build an image from a Dockerfile
      commit      Create a new image from a container's changes
      cp          Copy files/folders between a container and the local filesystem
      create      Create a new container
      diff        Inspect changes to files or directories on a container's filesystem
      events      Get real time events from the server
      exec        Run a command in a running container
      export      Export a container's filesystem as a tar archive
      history     Show the history of an image
      images      List images
      import      Import the contents from a tarball to create a filesystem image
      info        Display system-wide information
      inspect     Return low-level information on Docker objects
      kill        Kill one or more running containers
      load        Load an image from a tar archive or STDIN
      login       Log in to a Docker registry
      logout      Log out from a Docker registry
      logs        Fetch the logs of a container
      pause       Pause all processes within one or more containers
      port        List port mappings or a specific mapping for the container
      ps          List containers
      pull        Pull an image or a repository from a registry
      push        Push an image or a repository to a registry
      rename      Rename a container
      restart     Restart one or more containers
      rm          Remove one or more containers
      rmi         Remove one or more images
      run         Run a command in a new container
      save        Save one or more images to a tar archive (streamed to STDOUT by default)
      search      Search the Docker Hub for images
      start       Start one or more stopped containers
      stats       Display a live stream of container(s) resource usage statistics
      stop        Stop one or more running containers
      tag         Create a tag TARGET_IMAGE that refers to SOURCE_IMAGE
      top         Display the running processes of a container
      unpause     Unpause all processes within one or more containers
      update      Update configuration of one or more containers
      version     Show the Docker version information
      wait        Block until one or more containers stop, then print their exit codes

---------------------------------------------------------------------

### Naming conventions for images

- Image name needs to start with your account ID
- `zeeshanj/name-of-image`

- lets create an example of a new image with correct naming conventions
- `zeeshanj/sre_docker_app:v1`
- the `v1` tag specifies the `version` of the image, if no tag is included the version shall be known as `latest`

---------------------------------------------------------------------

## Run Dockerhub on localhost

- On the Terminal run this command `docker run -d -p 4000:4000 docs/docker.github.io`
- Then once downloaded run `localhost:4000` on a browser and you should be in dockerhub





