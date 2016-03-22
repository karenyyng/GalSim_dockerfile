# GalSim_dockerfile
Dockerfile for building [Galsim](https://github.com/GalSim-developers/GalSim).
The built image is hosted on [Dockerhub](https://hub.docker.com/r/karenyng/galsim_dockerfile/)
which is linked to this repo with a webhook, so any changes in the Dockerfile
in this repo will trigger a new build.

# How to use:

## Method 1: pull and run docker image 
1) Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads) if you do not have Linux as your OS.     
2) Install docker following [these
instructions](https://getcarina.com/docs/tutorials/docker-install-mac/).   
3) Start docker via the quickstart terminal.    
4) In the quickstart terminal with the whale logo, issue    
```
$ docker run -ti karenyng/galsim_dockerfile
```
then the image will be downloaded and run.
Press enter after the prompt does not change anymore and 
then you will have control of the container once the terminal prompt changes.
Press enter if nothing seems to happen after the download.


## Method 2: build and run docker image 
Using the dockerfile here and building the image will take much longer.
But you can do it if you want.
```
$ git clone https://github.com/karenyyng/GalSim_dockerfile.git
$ cd GalSim_dockerfile  # or whatever the folder name of the git repo is
```
Follow step 1-3 above, then
```
$ docker build -t IMAGE_NAME . 
```
You are free to choose what the `<IMAGE_NAME>` of the built image would be.
You can then run the built image by:
```
$ docker run -it IMAGE_NAME
```
