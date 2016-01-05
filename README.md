# PostgreSQL docker image based on Alpine Linux

This repo builds a docker image that accepts the same env vars as the
[official postgres build](https://registry.hub.docker.com/_/postgres/) but
with a much smaller footprint. It achieves that by basing itself off the great
[alpine](https://github.com/gliderlabs/docker-alpine) docker image by GliderLabs.

## Why?

```bash
$ docker images
REPOSITORY          TAG                 IMAGE ID            CREATED             VIRTUAL SIZE
alpine-postgres     latest              82d0ddb748fd        About an hour ago   23.87 MB
gliderlabs/alpine   3.3                 1e46923a8af6        12 days ago         4.794 MB
percona             latest              70588d0c4cd4        4 weeks ago         308.6 MB
postgres            latest              6d6a71f8528e        4 weeks ago         265.1 MB
```

# Build

```bash
$ make build
```

# License

MIT. See `LICENSE` file.
