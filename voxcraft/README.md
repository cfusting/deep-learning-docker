# Voxcraft-sim

## Installation instructions.

#### Requirements
When building voxcraft-sim the makefile checks if a GPU is available. Thus it is necessary for docker build to be able to see your GPU. To that end install and configure the [nvidia-container-runtime](https://stackoverflow.com/questions/59691207/docker-build-with-nvidia-runtime).

#### Build
```bash
cd voxcraft
docker build -t voxcraft-sim .
```

#### Run
```bash
docker run -it --gpus all voxcraft-sim
```
