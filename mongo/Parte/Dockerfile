FROM ubuntu:20.04

# Install MongoDB
RUN apt-get update && \
    apt-get install -y mongodb

# Create the MongoDB data directory
RUN mkdir -p /data/db

# Expose port #27017 from the container to the host
EXPOSE 27017

# Set /usr/bin/mongod as the dockerized entry-point application
ENTRYPOINT ["/usr/bin/mongod"]

VOLUME [ "/data/db" ]

#PRIMER CONTENDOR DOCKERFILE
# ejecutar esto
# sudo docker build -t mongo_dockerfile .
# sudo docker run -d -p27017:27017 --name monguito_dockerfile mongo

#SEGUNDO CONTENDOR  dockerrun
#docker run -d --name mongodockerun mongo:lastest

#TERCER CONTENEDOR
#El otro archivo el compose

#CUARTO CONTENEDOR O PRACTICA
#CREAR OTRO CONTENDOR
#docker run --name dockercommit -d mongo:latest
#docker commit dockercommit dockercommithijo
#docker run --name mimongocommit -d dockercommithijo
