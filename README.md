# Quartz Docker Image

Generates a docker image of Quartz and publishes the image to github.

## Usage

Quartz can now be run as a docker image, mounting the `content` and `public` folders for the input and output.

```
podman run --rm -it \
  -v $PWD/content:/usr/src/app/content \
  -v $PWD/public:/usr/src/app/public \
  ghcr.io/jamestalton/quartz \
  npx quartz build
```
