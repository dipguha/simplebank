# simplebank Application 

## Download Go from Go website

1.  go version from command prompt
    1. Edit .bash_profile
    2. source ~/.bash_profile
2.  Install VS Code
    1. Set code . (command shift P, shell command: Install code command in PATH)
    2. go run main.go
    3. Open Editor disable - Code - Settings - feature - explorer - open editors - 0

3. Install Docker and Database
    1. Install Docker desktop
    2. Install Table Plus
    3. DB name = root, select now();
4. Run Postgres Container
    1. docker pull postgres:12-alpine
    2. docker images
    3. docker run --name postgres12 -p 5432:5432 -e POSTGRES_USER=root -e POSTGRES_PASSWORD=secret -d postgres:12-alpine
    4. docker exec -it postgres12 psql -U root
    5. docker logs postgres12
5. Create DB schema


