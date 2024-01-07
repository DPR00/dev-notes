# Examples on how to run a container

This is an example on runing a container for orb_slam3. It contains more parameters to have in account. I put it here just as a note (doc for later).

```bash
# Create a new container
docker run -td --privileged --net=host --ipc=host \
    --name="orbslam3" \
    -e "DISPLAY=$DISPLAY" \
    -e "QT_X11_NO_MITSHM=1" \
    -v "/tmp/.X11-unix:/tmp/.X11-unix:rw" \
    -e "XAUTHORITY=$XAUTH" \
    -e ROS_IP=127.0.0.1 \
    --cap-add=SYS_PTRACE \
    -v `pwd`/ORB_SLAM3/Datasets:/Datasets \
    -v /etc/group:/etc/group:ro \
    -v `pwd`/ORB_SLAM3/ORB_SLAM3:/ORB_SLAM3 \
    jahaniam/orbslam3:ubuntu20_noetic_cpu bash
```
