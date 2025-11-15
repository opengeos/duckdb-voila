---
title: DuckDB Voila
emoji: 🚀
colorFrom: red
colorTo: red
sdk: docker
app_port: 7860
tags:
  - leafmap
pinned: false
short_description: A Voila template for DuckDB
license: mit
---

# duckdb-voila

Build a docker image for using DuckDB with Voila

To build the image:

```bash
docker buildx build --platform linux/amd64,linux/arm64 -t giswqs/duckdb:voila --push .
```

To run the image:

```bash
docker run -it -p 7860:7860 -v $(pwd):/home/jovyan/notebooks giswqs/duckdb:voila
```

To push the image to the registry:

```bash
docker push giswqs/duckdb:voila
```
