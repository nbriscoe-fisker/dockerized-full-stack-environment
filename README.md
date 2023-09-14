# Dockerized Full-Stack Environment

## Folder structure

```
📦dockerized-full-stack-environment
 ┣ 📂mysql-db
 ┃ ┣ 📜00-create-db.sql
 ┃ ┣ 📜01-create-table-users.sql
 ┃ ┗ 📜02-populate-users-table.sql
 ┣ 📂nestjs-app
 ┃ ┣ 📂node_modules
 ┃ ┣ 📂src
 ┃ ┣ 📂test
 ┃ ┣ 📜.dockerignore
 ┃ ┣ 📜Dockerfile
 ┃ ┣ 📜package.json
 ┃ ┗ 📜webpack-hmr.config.js
 ┣ 📂nextjs-app
 ┃ ┣ 📂node_modules
 ┃ ┣ 📂pages
 ┃ ┣ 📂public
 ┃ ┣ 📂styles
 ┃ ┣ 📜.dockerignore
 ┃ ┣ 📜Dockerfile
 ┃ ┣ 📜package.json
 ┃ ┗ 📜next.config.js
 ┣ 📜.env
 ┣ 📜docker-compose.yml
 ┗ 📜package.json
 ```

## Install Docker Desktop

- <https://docs.docker.com/desktop/install/windows-install/>
- <https://docs.docker.com/desktop/install/linux-install/>
- <https://docs.docker.com/desktop/install/mac-install/>

## Run everything together

Run `docker-compose up`

## Run projects separated

### Run the mysql-db

`npm run start:db` or `docker-compose up mysql-db`

### Run the nestjs-app

`npm run start:back` or `docker-compose up nestjs-app`

### Run the nextjs-app

`npm run start:front` or `docker-compose up nextjs-app`

### Clean the database volume

Run `npm run clean` or `docker-compose down -v`

## Credit

The boilerplate for this technical question came from [GustavoContreiras/dockerized-full-stack-environment](https://github.com/GustavoContreiras/dockerized-full-stack-environment)

## Useful links

- <https://nextjs.org/docs/getting-started>
- <https://docs.nestjs.com/first-steps>
- <https://docs.nestjs.com/recipes/hot-reload>
- <https://docs.nestjs.com/recipes/sql-typeorm#sql-typeorm>
- <https://docs.nestjs.com/techniques/database>
