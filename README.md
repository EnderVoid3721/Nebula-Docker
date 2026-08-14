# Nebula-Docker
An easy to use docker image for hosting Nebula Proxy in docker, without having to install dependencies or or build from a docker image, in case your server is using a partially read only file-system like Zima OS (My server)<br>

This Repository does not yet garuntee support for Marketplace or Games, only the Proxy Service.

This Repository uses [```elijahn372/nebula-docker```](https://hub.docker.com/layers/elijahn372/nebula-docker/v2.0/images/sha256:43c968f092525a6e05362fa207ceb2a873bdb79d5ac515ea41f0175d49e6c626?uuid=852F6A3F-AAA3-4DAB-8EC3-4D3D18C87DA1) from Docker Hub

This will not always have the most up to date Nebula version or its dependencies. It is recommended that you try to follow the instructions on the original github if it is possible for you.  
[Original GitHub](https://github.com/NebulaServices/Nebula)

## Prerequisites/Dependencies

 1. Git (you could also download the Repository ZIP file, and extract it, if able to)
 2. Docker
 3. ```Sudo``` has been added to some commands, as some Server OS's have more restrictions, and it may be necessary, but you can remove it if it isn't needed

## Installation/Setup
 - Clone the Repository
 ```sudo git clone https://github.com/EnderVoid3721/Nebula-Docker && cd Nebula-Docker```

 - Make the config file
 ```cd ./nebula/nebula```
 ```sudo cp config.example.toml config.toml``` 
 - Edit your configurations
 ```sudo nano config.toml```

## Docker compose

 - For ZimaOS
 ```cd ZimaOS```
 ```sudo docker up```
  - For Other Server Type/OS
 ```cd Generic```
 ```sudo docker up```

## Docker CLI
 - Pull the Image
 ```sudo docker pull ```
  - Start the Image in a container
 ```sudo docker run -d -p 5377:8080 -v ./nebula:/data elijahn372/nebula-docker:v2.0```

<h3>Nebula should now be running on port 5377</h3>

 - You can change your port from the ```compose.yaml``` file in ZimaOS or Generic Directory, or change the **5377** in your ```docker run``` command for Docker CLI

If you have any questions, I am most likely to respond on [Discord](https://discord.com/users/888835513933496402)


