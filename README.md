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
* may/25/2020
* 

# nginx log
* The nginx_main_site.conf
*	the fist block hte server is created and listens on port 80 rooted in the services folder under www within html
*	 /srv/www/html on the image.
* the second block: requires changing for bigger sites, but essentially prevents the download of '.'files such as
*	.htaccess, .htpasswd and others that should not be publicly available 
* the last block: makes sure that any path starting with '/' will be read from root and 
*	if the index file is not provided, will use the internal index.html.
*	if none available in the directory the autoindex ensures that it can show you a human listing of a directory.
* 
* the nginx confi is functional, but does not include ssl/ loggin/ error files/ file lookup/ matching ....est...
*

