# simplebank Application 

1.  Install Go
    1. go version (go version go1.17.7 darwin/amd64)
    2. go env GOPATH (/Users/cguha/go)
    3. Edit .bash_profile, export PATH=$PATH:$(go env GOPATH)/bin
    4. source ~/.bash_profile
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
5. Migration library
    - brew install golang-migrate
    - migrate -version
    - migrate help
    - migrate create -ext sql -dir db/migration -seq init_schema
6. CRUD library
    - DATABASE/SQL low level package as part of Go
    - GORM
    - SQLX library
    - SQLC, our prefered method
        - brew install sqlc
        - sqlc version (v1.24.0)
        - brew list. brew uninstall sqlc
        - brew install kyleconroy/sqlc/sqlc
        - sqlc init
    - go mod init github.com/dipguha/simplebank
    - go mod tidy


