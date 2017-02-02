# Dockers, Vagrant and Nodejs
 
 #Synopsys
 
 Virtual Machine for develop environment using:
 - Dockers Containers
 - NodeJs
 - ExpressJs
 - MongoDb
 - Redis
 - Nginx
 - Mysql
 
 #Installation 
- Install vagrant: using http://vagrantup.com/downloads.html
- Install the Vagrant Provisioner: Docker Compose

```bash
    vagrant plugin install vagrant-docker-compose
```

- clone this repo
- copy the file docker-compose.yml.example
```bash
cp /path_of_the_project/docker/docker-compose.yml.example /path_of_the_project/docker/docker-compose.yml
cp /path_of_the_project/app/.env_example /path_of_the_project/app/.env
```
- enjoy your docker virtual machine!!!
