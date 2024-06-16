Image# Ubuntu 24.04 LTS Ansible Test Image

[![Publish Image](https://github.com/MonolithProjects/docker-systemd-ubuntu24/actions/workflows/publish.yml/badge.svg)](https://github.com/MonolithProjects/docker-systemd-ubuntu24/actions/workflows/publish.yml)
[![DockerHub-pulls](https://img.shields.io/docker/pulls/monolithprojects/systemd-ubuntu24)](https://hub.docker.com/repository/docker/monolithprojects/systemd-ubuntu24)
[![DockerHub](https://img.shields.io/docker/image-size/monolithprojects/systemd-ubuntu24)](https://hub.docker.com/repository/docker/monolithprojects/systemd-ubuntu24)

Docker image with Ubuntu 24.04 LTS and enabled systemd. Image contains also `ansible` user (UID/GID 1000) with NOPASSWD:ALL sudo rights.  
This docker image is ment to be used for development purpose. I do not recomend to use it in production.

## Tags

- `latest`  
- `<monthly build timestamp>` for the list of the tags see the [Docker Hub](https://hub.docker.com/repository/docker/monolithprojects/systemd-ubuntu24/tags?page=1)

## How-to

  1. Pull image with command `docker pull monolithprojects/systemd-ubuntu24:latest`  
  2. Run the container from the image: `docker run --detach --privileged --volume=/sys/fs/cgroup:/sys/fs/cgroup:ro monolithprojects/systemd-ubuntu24:latest`  

## License

MIT
