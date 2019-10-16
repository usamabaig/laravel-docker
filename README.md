<p align="center">
    <img src="/.github/home-page-images/laradock-logo.jpg?raw=true" alt="Laradock Logo"/>
</p>

---

<p align="center"><b>Full PHP development environment based on Docker.</b></p>

<p align="center">Supporting a variety of common services, all pre-configured to provide a full PHP development environment.</p>

<p align="center">
   <a href="http://laradock.io/contributing"><img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat" alt="contributions welcome"></a>
   <a href="https://github.com/laradock/laradock/network"><img src="https://img.shields.io/github/forks/laradock/laradock.svg" alt="GitHub forks"></a>
   <a href="https://github.com/laradock/laradock/issues"><img src="https://img.shields.io/github/issues/laradock/laradock.svg" alt="GitHub issues"></a>
   <a href="https://github.com/laradock/laradock/stargazers"><a href="#backers" alt="sponsors on Open Collective"><img src="https://opencollective.com/laradock/backers/badge.svg" /></a> <a href="#sponsors" alt="Sponsors on Open Collective"><img src="https://opencollective.com/laradock/sponsors/badge.svg" /></a> <img src="https://img.shields.io/github/stars/laradock/laradock.svg" alt="GitHub stars"></a>
   <a href="https://travis-ci.org/laradock/laradock"><img src="https://travis-ci.org/laradock/laradock.svg?branch=master" alt="Build status"></a>
   <a href="https://raw.githubusercontent.com/laradock/laradock/master/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="GitHub license"></a>
</p>

<p align="center">
    <a href="http://zalt.me"><img src="http://forthebadge.com/images/badges/built-by-developers.svg" alt="forthebadge" width="240"></a>
</p>



<h4 align="center" style="color:#7d58c2">Use Docker First - Then Learn About It Later</h4>

<p align="center">
	<a href="http://laradock.io">
	   <img src="https://raw.githubusercontent.com/laradock/laradock/master/.github/home-page-images/documentation-button.png" width="300px" alt="Laradock Documentation"/>
	</a>
</p>

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
