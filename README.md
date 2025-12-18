# Dockerfiles

## Build the ROS2 Jazzy img

```bash
docker build -t ros2:jazzy_cuda -f ./juzzy-cuda_v2.Dockerfile
```

## Run the img
```bash
docker compose -f jazzyCompose.yaml up -d
docker exec -it ros2_u24_cuda_dev bash
```
or
`dokcer run -it <docker_img_name> bash`
