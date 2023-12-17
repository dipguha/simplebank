# simplebank 1
## Download Go from Go website
## go version from command prompt
## Edit .bash_profile
## source ~/.bash_profile
## Install VS Code
## Set code . (command shift P, shell command: Install code command in PATH)
## go run main.go
## Open Editor disable - Code - Settings - feature - explorer - open editors - 0

## Install Docker and Database
### Install Docker desktop
### Install Table Plus
### DB name = root, select now();
### Run Postgres Container
### docker pull postgres:12-alpine
### docker images
### docker run --name postgres12 -p 5432:5432 -e POSTGRES_USER=root -e POSTGRES_PASSWORD=secret -d postgres:12-alpine
### docker exec -it postgres12 psql -U root
### docker logs postgres12
### Create DB schema
###

