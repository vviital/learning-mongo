# Summary

I use docker to load and run mongodb instance.

# Start container

First of all you should build your container with mongo. You can do it in this way:

```
sudo docker build -t vviital/mongo-db .
```

# Restore dump

Due to requirements of tasks of week-2, I should restore dump of movie database. For this purpose I should use mongorestore utility (dump is already loaded into container, see Dockerfile). Container id can be found by running command ```sudo docker ps -a```

```
sudo docker exec :container-id mongorestore /home
```

# Connect to mongodb instance using mongo utility

```
sudo docker exec -it :container-id mongo
```
