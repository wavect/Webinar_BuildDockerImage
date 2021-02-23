1. Create angular project
`ng new wavect-docker`

2. Build Image
`docker build -t angulartest .`

3. Run Image
`docker run --name wavect -d -p 8080:80 angulartest`

If you are using Docker Toolbox, you may want to use this ip instead of localhost: 
`docker-machine ip`