#h2 database
docker build --no-cache -t mcerovski/h2database:latest .

docker run -it -p 9092:9092 -p 8082:8082 mcerovski/h2database -tcpAllowOthers -webAllowOthers

You can access to http://localhost:8082/ to see Web console.