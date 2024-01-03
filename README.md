Install and Set Up Laravel with Docker Compose
Setting up Laravel in the local environment with Docker using the LEMP stack that includes: Nginx, MySQL, PHP,

Why use Docker for Development

 Consistent development environment for the entire team.
 You don't need to install a bunch of language environments on your system.
 You can use different versions of the same programming language.
 Deployment is easy

 
How to Install and Run the Project
git clone git@github.com:hanieas/Docker-Laravel.git
docker-compose exec app composer install
Copy .env.example to .env
docker-compose build
docker compose up -d
You can see the project on 127.0.0.1:8080
How to use MySQL as a database
Uncomment the MySQL configuration inside the docker-compose.yml including: db and phpMyAdmin
Copy .env.example to .env
Change DB_CONNECTION to mysql
Change DB_PORT to 3306
Open the phpMyAdmin on 127.0.0.1:3400
