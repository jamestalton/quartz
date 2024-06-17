# Quartz Docker Image

Generates a docker image of Quartz and published the image to github.

```
podman run --rm -it -v $PWD/docs:./docs -v $PWD/public:./public ghcr.io/jamestalton/quartz npx quartz build -d docs
```
