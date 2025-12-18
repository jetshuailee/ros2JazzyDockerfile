# Dockerfiles

## Build the ROS2 Jazzy img

```bash
docker build -t ros2:<Tag> -f ./juzzy-cuda_v2.Dockerfile
```

## Run the img
```bash
docker compose -f <compose_file_path> up -d
docker exec -it <container_name>
```
or
`dokcer run -it <docker_img_name>`
