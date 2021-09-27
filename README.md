# Docker_intro

Create a github repo with a readme on how to set up docker, and 
what is docker benefits etc. , what is the microservices architecture, differences between
microservices and monolith architecture, differences between vm and docker. Tomorrow standup 9:30, do this before then

-----------------------------

## What is Docker

A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. A Docker container image is a lightweight, standalone, 
executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.

Docker images contain all the dependencies needed to execute code inside a container, so containers that move between Docker environments with the same OS work with no changes. 
Docker uses resource isolation in the OS kernel to run multiple containers on the same OS.

Docker is a set of platform as a service products that use OS-level virtualization to deliver software in packages called containers. 
Containers are isolated from one another and bundle their own software, libraries and configuration files; they can communicate with each other through well-defined channels



---------------------------------

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


---------------------------------------------

## What are microservices


----------------------------------------------

## Differences between microservices and monolith architecture
![image](https://user-images.githubusercontent.com/88186084/134947859-4e03bd56-81a2-4713-97ed-a216810dd2db.png)


------------------------------------------

## Differences between VM and Docker


-----------------------------------------------

## Docker Setup


--------------------------------------------------------






