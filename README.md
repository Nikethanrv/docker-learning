# docker-learning
### What is Docker?
Let's say we an application that needs a specific version of runtime environment, thats different from the host environment.
Docker isolates applications into containers, solving the problem of "BUT IT RUNS ON MY COMPUTER"

### What is an Docker Image?
Docker image contains all the neccessary details, metadata for the docker container to run.

### Volume
Is used for persistent storage of data outside the container

docker rm `docker ps -aq` --> To remove docker images

### Data Pipeline
A data pipeline produces some output for an input
                          -> Parquet File (stores data in binary)
CSV File -> Data Pipeline -> PostgreSQL Database
                          -> Data warehouse

# docker build -t test:pandas -> Building a docker image

# docker run test:pandas -> Running a docker container from the image