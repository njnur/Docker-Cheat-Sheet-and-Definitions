**Docker:** Docker is a set of platform as a service products that use OS-level virtualization to deliver software in packages called containers.

**Container:** A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another.

**Image:** A Docker container image is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.

**```docker run hello-world```**

When this command executes there happens a series of actions:
1. Docker cli receives the command and goes into Docker server
2. Docker server looks into Local Image cache
3. If there is no previous image of "hello-world" then it downloads the image from Docker Hub
4. Afterwards Docker server creates container from the images and loads and run the container

 