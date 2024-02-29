
# Dockerized Odoo 17 with PostgreSQL and PgAdmin

This is a flexible and  **streamlined**  version of most dockerized Odoo projects that you'll find. And one that allows you to deploy with two different methods using the same Dockerfile:

- **Standalone**: As most people use their implementation. With Odoo's ready image from Dockerhub and the source code is inside the container.  **This is the default**
-   **Hosted**: A more practical deployment for  **development**, as the HOST (where docker is installed) has the source code, and each container uses this single source.
-  **Source Code**: A more practical deployment for  **development**, as the HOST (where docker is installed) has the source code, and each container uses this single source.
-  **Module Directory**: For extend the Odoo functionality there is a **Extra Module Folder** to add the modules.
-  **Config file**: To configure the Odoo, we use the **odoo.conf** instead of docker environment.



## Requirements

[](https://github.com/iterativo-git/dockerdoo#requirements)

To use this docker compose file you should comply with this requirements:

-   Install  [Docker Desktop](https://www.docker.com/products/docker-desktop)  for Windows/Mac or  [Docker Engine](https://docs.docker.com/install/linux/docker-ce/ubuntu/#install-docker-ce)  for Linux
-   Install  [docker-compose](https://docs.docker.com/compose/install/)  (This is installed by default on Windows and Mac with Docker installation)
-   clone this repository  `git@github.com:iterativo-git/dockerdoo.git`

## Running 

```
git pull git@github.com:nimaam/Odoo_dockers.git
#Edit the PGAdmin and Postgresql with IP addresses
vi docker-compose.conf
##Add the database credentials 
vi data/odoo.conf
docker-compose up -d
```
