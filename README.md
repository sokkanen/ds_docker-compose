Docker-compose for a distributed system
=
This application is a part of academic work, demonstrating a distributed system.

You need to have Docker & Docker-compose installed in order to use this configuration.

NOTE: Not secure, work in progress.
--

Docker-compose setting for running a webshop.

Instructions:

1. Clone and build Inventory image from the respective repository
- https://github.com/sokkanen/Inventory

 ```
    $ mvn clean verify
    $ docker build -t inventory:latest .
 ```

2. Clone and build order image from the respective repository
- https://github.com/apndx/Order


3. Clone and build frontend image from the respective repository

 - https://github.com/vsvala/OnlineStore_back
 - https://github.com/vsvala/OnlineStore (this does not need it's own image, as it is included in OnlineStore_back)

4. Run application
 ```
    $ docker-compose up
 ```

5. Now you can open the Online Store with your [browser](http://localhost:3002). To simulate multiple customers, you can open the Online Store for example in two different browsers.
