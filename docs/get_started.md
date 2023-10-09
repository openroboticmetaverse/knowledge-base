# Get Started

Welcome to the starting point of your journey into the world of autonomous robots with ROS and Gazebo. Before you dive into creating and simulating robots, there are some prerequisites and tools you need to have in place. This guide will walk you through them.

## Prerequisites
!!! info "Supported Versions"
    This guide specifically covers the setup for ROS Humble on Ubuntu 22.04 LTS. If you're using different versions, please refer to the official ROS documentation for the appropriate setup instructions.

### 1. **Operating System**

- **Ubuntu**: ROS and Gazebo are primarily developed and tested on Ubuntu. For ROS Humble, it's recommended to use Ubuntu 22.04 LTS.

### 2. **Knowledge Base**

- **Programming**: Familiarity with programming, especially in Python and C++, will be highly beneficial.
- **Linux**: Basic knowledge of the Linux command line, as ROS relies heavily on it for its tools and utilities.

### 3. **Hardware Requirements**

- **Processor**: A multi-core processor, 2 GHz or faster.
- **RAM**: At least 8 GB of RAM (16 GB recommended for smoother performance).
- **Graphics**: Dedicated GPU is recommended for rendering complex simulations in Gazebo.

## Installation Steps

### 1. **Setup Sources and Keys**

```bash
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
```

!!! warning "Avoid Multiple ROS Versions"
    Installing multiple versions of ROS on the same system can lead to conflicts. If you already have another version of ROS installed, consider using a virtual machine or Docker container for ROS Humble.

### 2. **Install ROS Humble**

```bash
sudo apt update
sudo apt install ros-humble-desktop-full
```

### 3. **Initialize ROS**

```bash
sudo rosdep init
rosdep update
```

### 4. **Install Gazebo**

Gazebo usually comes bundled with the full installation of ROS. However, if you need to install it separately:

```bash
sudo apt install gazebo
```

## Next Steps

Once you've set up ROS Humble and Gazebo, you're ready to start creating and simulating robots! Here are some recommended steps to continue:

1. **Tutorials**: Start with the official [ROS Tutorials](http://wiki.ros.org/ROS/Tutorials) and [Gazebo Tutorials](http://gazebosim.org/tutorials) to understand the basics.
2. **Workspace Setup**: Create and manage your [ROS Workspace](http://wiki.ros.org/catkin/Tutorials/create_a_workspace).
3. **Community**: Join the ROS community forums and Gazebo community to ask questions, share projects, and collaborate.

!!! success "Good job"
    You've made it through the first step!
