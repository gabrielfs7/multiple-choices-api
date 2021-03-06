# Multiple Choice Api

A PHP implementation of a question and multiples choices Api.

## Getting Started

### Prerequisites

Before start, you must have installed in your machine the following tools:

* [Docker](https://docs.docker.com/engine/installation/) - version >=17.0
* [Docker Compose](https://docs.docker.com/compose/install/) - version >=1.18.0
* [Git](https://git-scm.com/)

### Installing

Follow the steps bellow to get the development/testing environment up and running:


1- Clone this repository:

```shell
git clone https://github.com/andreluizmachado/multiple-choices-api.git
```

2- Go to project folder:
```shell
cd multiple-choices-api
```

3- Install the dependencies:
```shell
composer install
```
4- Create your .env file:
```shell
cp .env.dist .env
```

5- Start the application:
```shell
docker-compose up -d
```

6- Access the bellow address in your browser:
```shell
curl http://localhost:8080/questions?lang=en
```

## API Resources
Please check the [open-api.yaml](https://github.com/andreluizmachado/multiple-choices-api/blob/master/public/open-api.yaml) file into this project

## Running the tests

* **Unit and Functional tests** - After the docker-composer up, run the command:

```shell
 docker-compose exec -T multiple-choice-api ./vendor/bin/phpunit  
```
