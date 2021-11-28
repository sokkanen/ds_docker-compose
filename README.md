Docker-compose for a distributed system
=

Docker-compose setting for running a webshop.

Instructions:

1. Build inventory image from the respective repository:

    $ mvn clean verify
    $ docker build -t inventory:latest .

2. Build order image from the respective repository (Not implemented yet)

3. Build frontend image from the respective repository (Not implemented yet)

4. Run application

    $ docker-compose up

Inventory should now be load-balanced and available at localhost:9000