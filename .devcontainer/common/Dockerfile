ARG ROS_DISTRO

FROM ros:${ROS_DISTRO}

# Create a workspace
RUN mkdir -p /root/ws/src

# Install demo pkgs
RUN apt update && \
    apt install \
    ros-humble-rviz2 \
    ros-humble-rosbridge-server \
    ros-humble-navigation2 \
    ros-humble-nav2-bringup \
    ros-humble-turtlebot3-gazebo \
    -y

# Add sources to bashrc
RUN echo "source /opt/ros/humble/setup.bash" >> ~/.bashrc && \
    echo "source /usr/share/gazebo/setup.bash" >> ~/.bashrc && \
    echo "export TURTLEBOT3_MODEL=waffle" >> ~/.bashrc && \
    echo "export GAZEBO_MODEL_PATH=$GAZEBO_MODEL_PATH:/opt/ros/humble/share/turtlebot3_gazebo/models" >> ~/.bashrc