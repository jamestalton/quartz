# Quartz Docker Image

Generates a docker image of [Quartz](https://quartz.jzhao.xyz/) and publishes the image to github.

## Usage

Quartz can now be run as a docker image, mounting the `content` and `public` folders for the input and output.
It can be configures by mounting a `quartz.config.ts`.

```
podman run --rm -it \
  -v ./content:/usr/src/app/content \
  -v ./public:/usr/src/app/public \
  -v ./quartz.config.ts:/usr/src/app/quartz.config.ts \
  ghcr.io/jamestalton/quartz \
  npx quartz build
```
