Postgresql

You need a ```.env``` file to set the required parameters.  It should look like this:

```bash
COMPOSE_PROJECT_NAME=postgresql_latest # this should be unique for every version of postgres since the data volume will be persisted and will be named based on this value.
POSTGRES_VERSION=latest # the container version you want to use
POSTGRES_USER=YourUserNameHere
POSTGRES_PASSWORD=YourUserPasswordHere

ADMINER_PORT=8080 # the port to run the admin interface on
```


Run ```docker-compose up``` to start the container.

Browse to http://localhost:8080 to view the database where 8080 is the ADMINER_PORT
