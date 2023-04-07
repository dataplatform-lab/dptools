# How to

## Prerequisites

Use docker-container driver for multi-target build

```bash
docker buildx create --name multi-builder --driver docker-container --bootstrap
```

## Build and push dockerfiles

```bash
docker buildx build -t dataplatformlab/jupyterlab --platform linux/amd64,linux/arm64 --push .
```
