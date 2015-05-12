docker-images
=============

Build files for Docker images

What's here:

* A vagrant-friendly Debian Wheezy image

To use these images (see https://hub.docker.com/u/iven/):

```bash
$ docker pull iven/<image-name>:<tag>
```
To build these images:

```bash
$ docker build -t my_image_name <path/to/Dockerfile>
```
