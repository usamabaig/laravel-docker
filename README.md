# Laradock for Laravel
> This repo is inspired by and forked from "https://github.com/laradock/laradock".

---

## Setup

1) Make sure that you have windows 10 pro or ultimate installed and Virtualization enabled (from bios)
2) Download and Install docker for windows and switch to linux containers (by right click on docker icon in taskbar)
3) Go to laravel project folder and clone the following repository: https://github.com/usamabaig/laravel-docker
4) Go to newly created "laradock" folder in project folder and change env.example to .env
5) Change PHP_VERSION value to "your desired PHP version e.g 7.1" and MYSQL_VERSION to "your required MySql version e.g 5.7"
6) In terminal, go to laradock folder and run this command "docker-compose up -d nginx mysql phpmyadmin redis workspace" (Wait for the command to finish)
7) Open .env of laravel project and change DB_HOST value to "mysql" and REDIS_HOST value to "redis"
8) Run "Docker ps" command and make sure that all containers are up and running
9) Open browser and type your project folder name in url and Voila your project is served on docker

> If facing issues, you can check logs of any container by this command "docker logs CONTAINER_NAME e.g docker logs mysql"

## License

[MIT License](https://github.com/laradock/laradock/blob/master/LICENSE)
