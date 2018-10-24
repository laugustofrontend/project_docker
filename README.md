# Base design with docker

> created project base with containers in docker

## Stack Project
- Docker
- PHP 5.6-FPM
- MySQL
- Nginx
- PhpMyAdmin

## Project Structure
    .
    |__ nginx/
    |   |__ default.conf
    |   |__ Dockerfile
    |__ php/
    |   |__ Dockerfile
    |__ www/
    |   |__ html/
    |__ .env.example
    |__ CONTRIBUTING.md
    |__ docker-compose.yml
    |__ docker-start-container.sh
    |__ docker-stop-container.sh
    |__ LICENSE.MD
    |__ README.md

## Run project locally based debian
**1 -** Prepare the environment
```sh
$ sudo curl -sSL https://get.docker.com | sh
```
**2 -** ADD your use in group docker
```sh
$ sudo chmod -aG docker username
```
**3 -** Install docker compose
```sh
$ curl -L https://github.com/docker/compose/releases/download/1.15.0/docker-compose-linux-x86_64 -o /usr/local/bin/docker-compose
$ sudo chmod +x /usr/local/bin/docker-compose
```
**4 -** Restart your PC
```sh
$ shutdown -r now
```

After all the above steps enter into **.env** file and change the values variables for your project.

**5 -** Execute the docker-compose
```sh
$ docker-compose up -d
```
