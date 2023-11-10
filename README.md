# Nathan-Mer-Mongo
Tiny git repo with a Dockerfile to start mongo

Docker commands needed for this service

First build the docker image

```bash
docker build -t nathan-mongo-image .
```

Then run the docker container

```bash
docker run -d -p 27017:27017 --name nathan-mongo nathan-mongo-image
```

```bash
mongo --host localhost --port 27017
```

Once the mongo container is up and running, you can either view the contents using mongo shell or through a gui such as mongo compass, https://www.mongodb.com/try/download/compass. 