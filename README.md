# LearningDocker
starting to learn docker.  

# May 2020 log:
* The FROM line. 
*	FROM ubuntu:lastest - indicates the latest ubuntu docker image as the base to run the service
*	this image will pull from docker hub but the image can also be from a customer repo.
* The RUN line.
*	RUN will install some packages, we can define any packages we want, such as python.
*		other tools we want to install and services we want. 
*		here the ping utility is installed, all done through the ubuntu package manager apt, via apt-get cmd
* The CMD line.
*	CMD will instruct docker that by default, docker will run ping [web page] every time the container is started without further arguments.
* 
