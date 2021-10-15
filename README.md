
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)


# Service Connector Template

<p align="center">
  <img src="https://user-images.githubusercontent.com/20951805/137320834-c8f65e69-9aa8-45b7-9652-c359fd8cfd78.png" alt="Service Connector logo" height="250px"/>
</p>

This is a template for using the [service-connector](https://www.npmjs.com/package/service-connector) npm package that allows to easily create a service connect different clouds, databases, APIs, services, and others.

The source code and documentation is available in [Service-Connector-Core](https://github.com/unparallel-innovation/Service-Connector-Core).


## Quick Start
You need to be logged in to use the [template](https://github.com/unparallel-innovation/Service-Connector-Template/generate) to create your own Service Connector repository.

It is also possible to clone this repo to test and see how it works before using the template.

Run the Service Connector with:
```
node start.js
```
or
```
./start.sh
```


## Docker
Use the included Dockerfile to create a docker image and run it.
```
docker build -t service-connector . --no-cache
docker run -d service-connector
```
Check if the container if running and see the output.
```
docker ps
docker logs <CONTAINER-ID>
```
To stop the container use:
```
docker stop <CONTAINER-ID>
```


### docker-compose
Use the included docker-compose.yml to run with docker-compose.
```
docker-compose -f docker-compose.yml up -d
```
Check if the container if running and see the output.
```
docker ps
docker logs <CONTAINER-ID>
```
Stop the Service Connector with:
```
docker-compose -f docker-compose.yml down
```


### docker stack
Use the included docker-compose.yml to create a docker stack.
```
docker stack deploy -c docker-compose.yml service-connector
```
Check if the container if running and see the output.
```
docker stack ls
docker ps
docker logs <CONTAINER-ID>
```
Stop the Service Connector stack with:
```
docker stack rm service-connector
```


## Related Repositories:
*  [Service-Connector-Core](https://github.com/unparallel-innovation/Service-Connector-Core)


## Getting Support
If you'd like to report a bug or a missing feature, please use [GitHub issue tracker](https://github.com/unparallel-innovation/Service-Connector-Template/issues).


## License
This software is free and is distributed under the [MIT License](https://opensource.org/licenses/MIT).
