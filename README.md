### Docker Terminologies

**Docker:** Docker is a set of platform as a service products that use OS-level virtualization to deliver software in packages called containers.

**Container:** A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another.

**Image:** A Docker container image is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.

**```docker run hello-world```**

When this command executes there happens a series of actions:
1. Docker cli receives the command and goes into Docker server
2. Docker server looks into Local Image cache
3. If there is no previous image of "hello-world" then it downloads the image from Docker Hub
4. Afterwards Docker server creates container from the images and loads and run the container

**Control Groups:** cgroups, which stands for control groups, are a kernel mechanism for limiting and measuring the total resources used by a group of processes running on a system. For example, you can apply CPU, memory, network or IO quotas.
cgroups were originally developed by Paul Menage and Rohit Seth of Google, and their first features were merged into Linux 2.6.24.

**Namespaces:** Namespaces are a kernel mechanism for limiting the visibility that a group of processes has of the rest of a system. For example you can limit visibility to certain process trees, network interfaces, user IDs or filesystem mounts.
Namespaces were originally developed by Eric Biederman, and the final major namespace was merged into Linux 3.8.

### Docker CheatSheet
* `docker create <image-name>` create a docker container
* `docker start -a <image-name/image-id>` start a docker container
* `docker run <image-name>` run an image
* `docker ps` list running containers
* `docker ps --all` list all containers
* `docker system prune` delete all containers
* `docker logs <container-id>` get container logs
* `docker stop <container-id>` stop containers
* `docker kill <container-id>` kill containers
* `docker exec -it <container-id> <command>` kill containers
 