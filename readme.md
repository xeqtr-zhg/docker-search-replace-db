# Docker image based on utility Search-Replace-DB

This build uses the on-the-fly generation method, that is, the image files are assembled at the time the main container is created.

We strongly recommend using docker-compose in combination, this is the most convenient and flexible method.

## Use with docker-compose

- Copy the "docker" folder of the current image to the root of the project

- Add a service call to your file docker-compose.yml

```
sr:
  build: ./docker/search-replace/
  ports:
    - '8055:80'
```

- start container generation
```

docker-compose build

```
- start the container

```
docker-compose up -d
```