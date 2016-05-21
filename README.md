# Mapbox Altas Server

## Download

Download the `linux` image for [Atlas Server](https://www.mapbox.com/studio/atlas) and unzip it.

## Set up Docker

```bash
$ docker build -t atlas .
```

## Run Atlas

```bash
$ docker run -d -p 2999:2999 --name atlas atlas
```

## Attach Data

Add a volume mount to your Docker run command `-v data:/opt/atlas-server-data/sources`.
