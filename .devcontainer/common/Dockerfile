ARG ROS_DISTRO

FROM ros:${ROS_DISTRO}

# Create a workspace
RUN mkdir -p /root/ws/src

# Install demo pkgs
RUN apt update && \
    apt install \
    ros-${ROS_DISTRO}-rviz2 \
    ros-${ROS_DISTRO}-rosbridge-server \
    ros-${ROS_DISTRO}-navigation2 \
    ros-${ROS_DISTRO}-nav2-bringup \
    ros-${ROS_DISTRO}-turtlebot3-gazebo \
    -y

# Add sources to bashrc
RUN echo "source /opt/ros/${ROS_DISTRO}/setup.bash" >> ~/.bashrc && \
    echo "source /usr/share/gazebo/setup.bash" >> ~/.bashrc && \
    echo "export TURTLEBOT3_MODEL=waffle" >> ~/.bashrc && \
    echo "export GAZEBO_MODEL_PATH=$GAZEBO_MODEL_PATH:/opt/ros/${ROS_DISTRO}/share/turtlebot3_gazebo/models" >> ~/.bashrc