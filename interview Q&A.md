1. What is Docker?
Docker is an open source containerization platform. It enables developers to package applications into containers.

2. What is difference between Containers and VM's ?
---Containers as very lightweight in nature because they don't have complete OS where it has very minimal system dependencies that required to run the application.
--In VM's we have full-fledged OS and hypervisor, making them heavier. VM's are less portable in nature. VM's have high level of security and can be isolated from host and other VM's.

3. What is docker lif cycle?
   Users would create Dockerfile with a set of instructions or commands that defines a docker image. For Eg, which base to use, what are the dependencies should be installed etc.
   Docker images act as a set of instructions to build a Docker container. It can be compared to a snapshot in a VM.
   Docker build ---->  docker pull ----> docker run ---->  docker push

4. What are the different docker components?
   Docker daemon is the heart of the docker. Docker daemon will understand the command we give in the CLI whether it may be run, pull etc. and does the work for us. Eg, if we give docker pull command deamon understand that image need to be pulled from the registry which may be private or docker hub.
![image](https://github.com/user-attachments/assets/8be64203-0d8d-48d8-886b-bb85c6d6312d)
![image](https://github.com/user-attachments/assets/4e7a33be-c9e2-4d2f-bcfa-f889c03417e4)

   
