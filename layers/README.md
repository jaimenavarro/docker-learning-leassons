# Build docker image test
```bash
docker build . -f docker/Dockerfile -t test
docker history test
```

# Build docker image test1
This image has layer 5 updated, **so from that layer on the rest are updated**. 
```bash
docker build . -f docker1/Dockerfile -t test1
docker history test1
```

# Compare layers docker images
```bash
docker history test
docker history test1
```

# Clean tests
```bash
docker rmi test test1
```
