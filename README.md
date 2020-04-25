# Docker
Setting and running applications using Docker.
---
References:
* Template: ["Docker-composing" a Python 3 Flask App Line-by-Line](https://medium.com/bitcraft/docker-composing-a-python-3-flask-app-line-by-line-93b721105777)
* Additional: [How To Serve Flask Applications with uWSGI and Nginx on Ubuntu 18.04](https://www.digitalocean.com/community/tutorials/how-to-serve-flask-applications-with-uswgi-and-nginx-on-ubuntu-18-04)
* [Docker config](https://medium.com/bitcraft/docker-composing-a-python-3-flask-app-line-by-line-93b721105777)
* [support](https://medium.com/bitcraft/dockerizing-a-python-3-flask-app-line-by-line-400aef1ded3a)
---
### Projects
**1. How To Set Up Flask with MongoDB and Docker**

 App: [How-to-set-up-flask-with-mongodb-and-docker](https://www.digitalocean.com/community/tutorials/how-to-set-up-flask-with-mongodb-and-docker)
 
---
## Installing Docker into Linux- Ubuntu

 * Start: [https://docs.docker.com/engine/install/ubuntu/](https://docs.docker.com/engine/install/ubuntu/)
 * check if you have the OS requirements (Bionic) by running ```cat /etc/*release*``` on the terminal.
 * Uninstall old versions by running ```sudo apt-get remove docker docker-engine docker.io containerd runc```.
 * Set up the repository.Easier way to install docker is to go down to the bottom *Install using the convenience script*.
     - ```curl -fsSL https://get.docker.com -o get-docker.sh```
     - ```sudo sh get-docker.sh```
 * Check docker version by running ```sudo docker version``` command.
 * Run a simple container to ensure everything is running as expected: ```sudo docker run docker/whalesay cowsay Hello-World```     found in the docker hub ``https://hub.docker.com/r/docker/whalesay``.
 
 ### Installing docker compose
 
 * RUN ```sudo pip install docker-compose```
---
*NB: In computer networking, port forwarding or port mapping is an application of network address translation (NAT) that redirects a communication request from one address and port number combination to another while the packets are traversing a network gateway, such as a router or firewall.*

 ## NGINX 
```$ docker run --name mynginx -p 80:80 -d nginx```

    + ``mynginx`` is the name of the created container based on the NGINX image.

    + the ``-d`` option specifies that the container runs in detached mode: the container continues to run until stopped but does not respond to commands run on the command line.
    
    + the ``-p`` option tells Docker to map the ports exposed in the container by the NGINX image (port ``80``) to the specified port on the Docker host. The first parameter specifies the port in the Docker host, the second parameter is mapped to the port exposed in the container.
 
