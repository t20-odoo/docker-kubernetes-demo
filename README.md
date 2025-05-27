# docker-kubernetes-demo

## Dive Into Docker!

_Diffchecker -_ <https://www.diffchecker.com/>

_diagrams.net (formerly draw.io) -_ <https://www.drawio.com/>

_Awesome Screenshot -_ <https://www.awesomescreenshot.com/>

---

**What is docker?** - Docker is a platform or ecosystem around creating and running containers.

_Docker Client_ - Tool that we are going to issue commands to

_Docker Server_ - Tool that is responsible for creating images, running containers, etc

---

**Why use docker?** - Docker makes it really easy to install and run software without worrying about setup or dependencies.

---

**Container**

- A standardized unit of software
- A package of code and dependencies to run that code (e.g. Node.js code + the Node.js runtime)
- The same container always yields the exact same application and execution behaviour! No matter where or by whom it might me executed.
- Support for containers is build into modern operating systems
- Docker smiplifies the creation and management of such containers

---

**Why docker and containers?**

- We want to have the exact same environment for development and production -> this ensure that it works exactly as tested
- It should be easy to share a common development environment/setup with (new) employees and colleagues
- We dont want to uninstall and re-install local dependencies and runtimes all the time

---

**Virtual Machines vs Docker Containers**

_Virtual Machines/Virtual OS_: Summary

_Pros | Cons_

- Separated environments | Redundant duplication, waste of space
- Environment-specific configurations are possible | Performance can be slow, boot time can be long
- Environment configurations can be shared and reproduced reliably | Reproducing on another computer/server is possible but may still be tricky

---

**Containers vs Virtual Machines**

_Docker Containers | Virtual Machines_

- Low impact on OS, very fast, minimal disc space usage | Bigger impact on OS, slower, high disc space usage
- Sharing, re-building and distribution is easy | Sharing, re-building and distribution can be challenging
- Encapsulated apps/environments instead of whole machines | Encansulated whole machines instead of apps/environments

---

**Docker Setup**

_macOS / Windows_

- Requirements met
  - Install docker desktop
- Requirements not met
  - Install docker toolblx

_Docker Playground_

If you can't install Docker on your system, you can also look into this online playground: <https://labs.play-with-docker.com/>

---

**Docker Tools & Building Blocks**

- _Docker Engine_: The **core runtime** that builds and runs containers. It includes the Docker daemon (`dockerd`) and the CLI (`docker`).
- _Docker Desktop (Incl Daemon & CLI)_: An **all-in-one application** for Windows and macOS that provides:
  - Docker Engine
  - Docker CLI (`docker`)
  - Docker Daemon
  - GUI for managing containers, images, and settings
- _Docker Hub_: A **cloud-based registry** where users can find, share, and store container images.
- _Docker Compose_: A **tool to define and run multi-container** Docker applications using a YAML file (`docker-compose.yml`).

---

**Docker Commands**

`docker version`

`docker build .` - Builds a Docker image from the Dockerfile in the current directory.

`docker images` - Lists all Docker images stored locally on your system, showing details like repository, tag, image ID, and size.

`docker run imageID` - Starts a new container from the specified image.

`docker run -p 3000:3000 imageID` - Runs a container and maps port 3000 of the host to port 3000 of the container.

`docker ps` - Lists all currently running Docker containers.

`docker stop containerName` - Gracefully stops a running container by its name.

---

## Docker Images & Containers

**Image** - Single file with all the deps and config required to run a program.

**Container** - Instance of an image. Runs a program.

## Manipulating Containers with the Docker Client
