# Mapbox Altas Server

## Download

Download the `linux` image of [Atlas Server](https://www.mapbox.com/studio/atlas) and unzip it into the `atlas-server` folder.

## Source Data

Download the source data and place them into `atlas-server-data/sources`.

## Set up Docker

```bash
$ cd atlas-server
$ docker build -t atlas .
```

## Run Atlas

Execute these commands in the root directory `Atlas-Server`.

**Option 1**

```bash
$ docker-compose up
```

**Option 2**

```bash
$ docker run -d -p 2999:2999 -v $(pwd)atlas-server-data:/opt/atlas-server-data --name atlas atlas
```
