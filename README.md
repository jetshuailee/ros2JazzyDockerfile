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

## Test the Nav2 pkg, try following cmd:
`ros2 launch nav2_bringup tb4_simulation_launch.py slam:=True headless:=False`
or 
`ros2 launch nav2_bringup tb3_simulation_launch.py slam:=True headless:=False`
`tb4_*` may take longer time to load the Gazebo scene or fail to load, kill it if
it freeze.