# Build linux executable
`env GOOS=linux go build *.go`

# Build Docker-Image
`docker build -t test . && docker run test`