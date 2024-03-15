# Ticketing FEST
> A full-stack web application for event ticketing

[![en](https://img.shields.io/badge/lang-en-red.svg)](link)
[![pt-br](https://img.shields.io/badge/lang-pt--br-green.svg)](link)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
</br> Disponível em português ao clicar o escudo acima "pt-br".

## Live Preview
Access on: [Ticket-Fest]()

Note: this live preview uses Render's free instance for back-ending hosting. Because of that, requests will take up to 50 seconds after long periods of inactivity and until then the 
## Getting Started

Clone this repository to your local environment with

```
git clone git@github.com:FelipeAlvesLeao/Ticketing-FEST.git
```

### Front-end

Switch to the folder frontend/Ticketing-front-end and run the commands
```
npm install
npm run dev
```
The client-side view will now be running on ```http://localhost:5173/```.
### Back-end
#### Option 1:
Import the folder backend/ on your preferred Java IDE, select a Java 17 compatible JDK and run the archive while on the folder backend/ticketing/src/main/java/dominios/api/ticketing/
#### Option 2:
While on the backend/ folder, run the commands
```
mvn package
java -jar target/TicketingApplication.jar
```
Make sure that you're running this command while on a version of the Java 17 JDK.
## Built With

* [Spring](https://spring.io/) - Java framework for back-end
* [Maven](https://maven.apache.org/) - Dependency Management for back-end
* [React](https://react.dev/) - Javascript library for front-end
* [NPM](https://www.npmjs.com/) - Dependency Management for back-end
* [MongoDB](https://www.mongodb.com/) - Database software
* [Docker](https://www.docker.com/) - Back-end images
 * [JIB](https://github.com/GoogleContainerTools/jib/tree/master) - Creates docker images from Maven



## Authors

* **Bruno Vinicius** - *Web design and front-end implementation* - [brunoviniciusrv](https://github.com/brunoviniciusrv)
* **Cauã Rebelo** - *Back-end implementation* - [cauarebelo](https://github.com/cauarebelo)
* **Felipe A. Leão** - *Back-end and front-end implementation* - [FelipeAlvesLeao](https://github.com/FelipeAlvesLeao)
* **Giovanna Lyssa** - *Back-end implementation* - [GiovannaLyssa99](https://github.com/GiovannaLyssa99)
## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```
## Building
### Front-end:
Inside of frontend/Ticketing-front-end/ run the command 
```
vite build
```

### Back-end: 
Inside of backend/backend/ run the command 
```
./mvnw clean install jib:dockerBuild
```
This creates a Docker image of the back-end server.
To understand the command, adapt it to your needs and configure it to automatically upload to Docker image repositories, check the [Jib Maven docs](https://github.com/GoogleContainerTools/jib/tree/master/jib-maven-plugin).
## Deployment

### Front-end:
Deploy the build folder made on the "Building" section.
### Back-end: 
Deploy either the built project using your preferred IDE or the image of the project.
For the image, you can acquire it using the command:
```
docker pull felipealvesleao/ticket-fest
```
## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

[Deploying a Spring Boot Application with Docker Image on render.com](https://medium.com/@nithinsudarsan/deploying-a-spring-boot-application-with-docker-image-on-render-com-9a87f5ce5f72)

</br>
