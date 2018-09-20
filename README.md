# hasaltaiar/miniconda3:{tag}

This repository builds a base image that can be used for building IoT Edge modules using Python. 
It creates an image that's based on Ubuntu and it includes 2 main components: 

## Miniconda 
Miniconda is widely used for managing dependencies, python version, etc. Read more about Miniconda [here](https://conda.io/miniconda.html)

## Tini
Tini is a simple and lightweight way of initialising containers. You can read more about Tini [here](https://github.com/krallin/tini/)


## Get started
To pull the image you can just do so easily: 

```sh
docker pull hasaltaiar/ubuntu_miniconda3

# or just run it directly
docker run -it hasaltaiar/ubuntu_miniconda3
```

## Build

Args expected:

- `MINICONDA_VERSION`
  - The `MINICONDA_VERSION` will become the `TAG` for the docker build
- `TINI_VERSION`
  - Current release avaiable for direct download is `v0.16.1`

For a list of `MINICONDA_VERSION` numbers available, search the
[Miniconda3 repo](https://repo.continuum.io/miniconda/) for any versions. 
