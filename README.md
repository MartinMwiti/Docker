# Docker
Setting and running applications using Docker.
---
* [Docker config](https://medium.com/bitcraft/docker-composing-a-python-3-flask-app-line-by-line-93b721105777)
---
### Projects
**1. How To Set Up Flask with MongoDB and Docker**

 App: [Link](https://www.digitalocean.com/community/tutorials/how-to-set-up-flask-with-mongodb-and-docker)
 
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

 
 
