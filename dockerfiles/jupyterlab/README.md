# JupyterLab

## Build and push dockerfiles

```bash
docker buildx build -t dataplatformlab/jupyterlab --platform linux/amd64,linux/arm64 --push .
```

## Pull the built image from the registry

```bash
docker pull dataplatformlab/jupyterlab
```

## Run the pulled image

```bash
docker run -p 8080:8888 -it dataplatformlab/jupyterlab:latest
```
