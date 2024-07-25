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

5. What is difference between docker COPY and docker ADD ?
   Docker ADD can copy the files from a URL unlike docker COPY which can only copy files from host system into the container.

6. What is the difference between CMD and Entrypoint in Docker?
   CLI arguments using the Docker run command will override the arguments specified using the CMD instruction.
   Whereas ENTRYPOINT instruction in the shell form will override additional arguements provides using CLI parameters or even through the CMD commands.

7. What are the networking types in Docker and what is the default?
   The default networking in Docker is Bridge.
   However, you can change the default type and configure one of the
   1. Bridge
   2. Overlay
   3. Host
   4. MacVlan

8. Can you explain how to isolate networking between the container?
   We can create network and assign the container to the networks. So that container will isolated from bridge network.

9. What is a multi stage build in Docker?
    Multi stage build allows you to build your docker container in multiple stages allowing you to copy artifacts from one stage to other. The major advantage of this is to build light weight containers.

10. What are distroless images in Docker ?
    Distroless images contain only your application and its runtime dependencies with a very minimum operating system libraries. They do not contain package mangers, shells or any other programs you would expect to find in a standard Linux distribution. They are very small and lightweight images.

11. ![image](https://github.com/user-attachments/assets/aa1b597e-1734-44f0-a0a0-00ffbbd2cee0)

12. ![image](https://github.com/user-attachments/assets/c708ca8d-aa1b-4c7c-92f6-ed73ff996acc)


   
