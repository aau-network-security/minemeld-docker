# minemeld-docker

MineMeld inside a docker container.

Based on phusion baseimage-docker, inspired by @swannysec and @bilalbox


## with docker compose

You still here ? Suggested way to run this docker:

````
docker-compose up
````

## without docker-compose

This commands creates a new MineMeld container, stores all the data and config
in the directory /somewhere/minemeld/local and binds to port 8443:

````
docker run -it --tmpfs /run -v /somewhere/minemeld/local:/opt/minemeld/local -p 8443:443 jtschichold/minemeld
````
