# MINIO

## Build and push dockerfiles

```bash
docker buildx build -t dataplatformlab/minio --platform linux/amd64,linux/arm64 --push .
```

## Pull the built image from the registry

```bash
docker pull dataplatformlab/minio
```

## Run the pulled image

```bash
docker run -p 9001:9001 -it dataplatformlab/minio:latest
```

