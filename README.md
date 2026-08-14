# Nebula-Docker
An easy to use docker image for hosting Nebula Proxy in docker, without having to install dependencies or or build from a docker image, in case your server is using a partially read only file-system like Zima OS (My server)
Original GitHub: https://github.com/NebulaServices/Nebula

Docker Compose (Recommended)
  ZimaOS:
    Download or Copy the Docker Compose file from https://github.com/EnderVoid3721/Nebula-Docker/blob/main/ZimaOS/compose.yaml
  Generic/Other Server:
    Download or Copy the Docker Compose file from https://github.com/EnderVoid3721/Nebula-Docker/blob/main/Generic/compose.yaml
  Create a Directory and put the compose.yaml file in it,
  Alternatively, you can clone the repository with
    ```git clone https://github.com/EnderVoid3721/Nebula-Docker.git```
    ```cd Nebula-Docker```
    For ZimaOS
      Migrate to the ZimaOS Directory - ```cd ZimaOS```
    For other Server Type/OS
      Migrate to the Generic Directory - ```cd Generic```
  Run ```docker compose up```

Instructions for Docker CLI will soon be added
Alternative Readme.md files would be appreciated, I have no idea how to use Markdown
To clarify, I did not code this, I mostly got dependencies installed, and made this into a ready to use Docker Container, All coding and development was done by https://github.com/NebulaServices
