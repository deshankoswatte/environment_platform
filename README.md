# Environment Platform

## Module Core(contains the back-end functionalities).

The following instructions below will guide you through the process of setting up the back-end server in your local machine.

### Prerequisites

- Ballerina 1.2.x
- Docker

### How to Build?

To build the module execute the command:

```
./setup.sh
```

### Create a configuration file

Make a file named `ballerina.conf` in `core/resources`. You can refer the file `example.conf` located at `core/resources/` for more details. Then, update the created file with your preference of values.

### Run the module using docker

All the volumes and internal networking for mongodb container is set using the docker-composer. Please follow the following commands to build the image and run.

##### Build the image

```
docker-compose build
```

##### Run the image

```
docker-compose up
```

##### Terminate the docker container

- Press `Ctrl+C` to terminate the program.
- Run `docker-compose down` to stop your containers.

#### Develop and run using docker

When you develop a feature and run using containers. You have to build the jar files using `./setup.sh` and then you have to build and up the docker composer.

### Run the module locally

**Important** - Make sure that the configuration files are setup for your local machine.

To run the module,

- Execute the command `cd core` to navigate to the `core` module.
- Then, run the script using the command `./scripts/run-local.sh`.
