# Ticketing FEST
>   Uma aplicação web full-stack de criação e venda de tickets.

[![en](https://img.shields.io/badge/lang-en-red.svg)](https://github.com/FelipeAlvesLeao/Ticketing-FEST/blob/main/README.md)
[![pt-br](https://img.shields.io/badge/lang-pt--br-green.svg)](https://github.com/FelipeAlvesLeao/Ticketing-FEST/blob/main/README.pt-br.md)
[![Licença: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
</br> Also avaliable in english by clicking the "lang en" shield above.

## Demonstração
Acesso: [Ticket-Fest](https://fantastic-phoenix-5b20db.netlify.app/)

Nota: essa demonstração usa uma instância gratuíta de servidor provido pela Render. Por isso, solicitações ao servidor após um longo tempo de inatividade precisam esperar cerca de 50 segundos de reinicialização do servidor.
## Iniciando 

Clone esse repositório localmente com o comando
```
git clone git@github.com:FelipeAlvesLeao/Ticketing-FEST.git
```

### Front-end

Mude para a pasta frontend/Ticketing-front-end e execute os comandos
```
npm install
npm run dev
```
O aplicativo front-end estará rodando, por padrão, no endereço ```http://localhost:5173/```.
### Back-end
#### Opção 1:
Importe a pasta backend/ na sua IDE de preferência, selecione uma JDK de Java 17 e rode o projeto na pasta backend/ticketing/src/main/java/dominios/api/ticketing/
#### Opção 2:
Dentro da pasta backend/, rode os comandos
```
mvn package
java -jar target/TicketingApplication.jar
```
Para o Maven usar uma JDK do Java 17, a variável JAVA_HOME deve apontar para JDK 17.
## Construído usando

* [Spring](https://spring.io/) - Framework Java para o back-end
* [Maven](https://maven.apache.org/) - Gerência de dependências para o back-end
* [React](https://react.dev/) - Biblioteca javascript para o front-end
* [NPM](https://www.npmjs.com/) - Gerência de dependências para o front-end
* [MongoDB](https://www.mongodb.com/) - Software de banco de dados
* [Docker](https://www.docker.com/) - Contâinerização do back-end
 * [JIB](https://github.com/GoogleContainerTools/jib/tree/master) - Contâinerização do back-end



## Autores

* **Bruno Vinicius** - *Web design e implementação front-end* - [brunoviniciusrv](https://github.com/brunoviniciusrv)
* **Cauã Rebelo** - *Implementação back-end* - [cauarebelo](https://github.com/cauarebelo)
* **Felipe A. Leão** - *Implementação back-end e front-end* - [FelipeAlvesLeao](https://github.com/FelipeAlvesLeao)
* **Giovanna Lyssa** - *Implementação back-end* - [GiovannaLyssa99](https://github.com/GiovannaLyssa99)

## Testes

## Builds
### Front-end:
Dentro da pasta frontend/Ticketing-front-end/ , execute o comando
```
npm run build
```
O aplicativo resultante será a pasta dist/
### Back-end: 
Dentro da pasta backend/backend/ , execute o comando
```
./mvnw clean install jib:dockerBuild
```
Isso cria uma imagem Docker do back-end
Mais informações: [Jib Maven docs](https://github.com/GoogleContainerTools/jib/tree/master/jib-maven-plugin).

## Deploy

### Front-end:
Faça o deploy da pasta dist/ construída na sessão "Build".
Confira se o serviço de host usado suporta websites dinâmicos.

### Back-end: 
Faça o deploy do projeto construído pela IDE (pasta target) ou use a imagem docker do projeto.

A imagem pode ser adquirida usando o comando:
```
docker pull felipealvesleao/ticket-fest
```
Note que você deve preencher o arquivo ```application.yml``` com detalhes da sua própria instância de um banco de dados MongoDB.

## Licença

Esse projeto está licenciado na licença MIT - veja o arquivo [LICENSE.md](LICENSE.md) para mais detalhes.

## Reconhecimentos

[Deploying a Spring Boot Application with Docker Image on render.com](https://medium.com/@nithinsudarsan/deploying-a-spring-boot-application-with-docker-image-on-render-com-9a87f5ce5f72)

</br>

## Nota final

Esse projeto foi desenvolvido como um projeto de universidade em um repositório diferente e, após finalização, movido para uma nova repo com um novo nome e documentação apropriada.

Para acessar o repositório original, com histórico de commits e merge, acesse [esse link](https://github.com/FelipeAlvesLeao?tab=repositories)
