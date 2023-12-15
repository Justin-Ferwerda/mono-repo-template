## Welcome to the world of containerization!
This Template is a mono-repo for a full-stack application utilizing next.js for the frontend and Django on the back end. It also uses Firebase for authentication. It is containerized with [Docker](https://www.docker.com/why-docker/) to create a streamlined development environment for any workflow.

## Getting Started

### What is Containerization?
From [Docker's website](https://www.docker.com/resources/what-container/):

>A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. A Docker container image is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.

>Container images become containers at runtime and in the case of Docker containers – images become containers when they run on Docker Engine. Available for both Linux and Windows-based applications, containerized software will always run the same, regardless of the infrastructure. Containers isolate software from its environment and ensure that it works uniformly despite differences for instance between development and staging.

### Why use Docker for this purpose?

### Getting Started using Docker

```git clone git@github.com:Justin-Ferwerda/mono-repo-template.git```

You will need 2 .env files: one for front end, one for back end.

Create a .env for front end in ```/CLIENT``` and place the api keys according to the sample.env.

For BE .env, you can create a new django secret key with this command-

```python3 -c 'from django.core.management.utils import get_random_secret_key; print(get_random_secret_key())'```

You will place it into a .env file in ```/API```, according to the sample.env.

Then while in the root folder, this command:

```docker compose up```

The build process should take about two minutes, once the api and web services are up and running, navigate to localhost:3000 and you should be good to go!
