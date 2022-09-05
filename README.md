# training-postgresql
 Training code to run testing postgresql sever with pgadmin in NodeJS with Docker

## Requirements
 - Docker compose

## Steps
### 1. Clone the repository
```shell
git clone https://github.com/sebastianaf/training-postgresql
cd training-postgresql
```
### 2. Set environment variables
Create a `.env` from `.env.example` file in the root folder with all environment variables, this variables will be used by the containers, it need to be reached by `docker-compose.yml` file.

### 3. Change `training` and `postgresql` names [Optional]
It's recommend to change all the names (in `docker-compose.yml`) named with `org` and `project` with your own organization name and project name.

### 4. Run
```shell
docker compose -p training-posgresql up -d
```
After type and run the command go to `localhost:${PG_ADMIN_PORT}`