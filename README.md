# ros2-humble-wsl-setup-guide
A comprehensive guide and visual documentation for installing and configuring ROS 2 Humble on Windows using WSL 2. Created for Smart Methods  (AI Track ).

# ROS 2 Humble Setup & Configuration Guide

## Project Overview
This repository contains a comprehensive, step-by-step documentation and visual walkthrough for setting up and configuring **ROS 2 (Robot Operating System - Humble Hawksbill)** on a Windows environment using the Windows Subsystem for Linux (WSL 2) running Ubuntu. It covers everything from enabling core virtualization features in the BIOS to configuring the Linux environment and validating the final ROS distribution build.

> **Project Context:** This project was developed as part of the AI Track training program for **Smart Methods**.

---

## Step-by-Step Implementation Guide

### Phase 1: Enabling WSL & Virtualization
1. **Enable Virtualization:** Access the system BIOS during startup and ensure that *Virtualization Technology* is enabled.
2. **Install WSL via PowerShell:** Open PowerShell as an administrator and execute the automated installation command:
   ```powershell
   wsl --install

Phase 2: Ubuntu Linux Setup
Launch the installed Ubuntu distribution from the Start menu.

Create a default UNIX username and secure password when prompted.

Phase 3: Installing ROS 2 Humble
Update system packages and install necessary dependencies inside the Ubuntu terminal:

sudo apt update && sudo apt upgrade
sudo apt install software-properties-common curl
sudo curl -sSL [https://raw.githubusercontent.com/ros/rosdistro/master/ros.key](https://raw.githubusercontent.com/ros/rosdistro/master/ros.key) -o /usr/share/keyrings/ros-archive-keyring.gpg
echo "deb [arch=amd64 signed-by=/usr/share/keyrings/ros-archive-keyring.gpg] [http://packages.ros.org/ros2/ubuntu](http://packages.ros.org/ros2/ubuntu) jammy main" | sudo tee /etc/apt/sources.list.d/ros2.list > /dev/null
sudo apt update
sudo apt install ros-humble-desktop

Phase 4: Environment Configuration & Testing
Configure the environment variables and verify the successful installation of ROS 2:

echo "source /opt/ros/humble/setup.bash" >> ~/.bashrc
source ~/.bashrc
echo $ROS_DISTRO

Visual Documentation & Execution Screenshots
Here is the visual record of the installation and configuration process:

1. Initial WSL Installation Process
2. PowerShell Execution & Setup
3. Virtual Machine Platform Initialization
4. Progress Tracking
5. System Terminal Initialization
6. Package List Updates
7. Core Software Dependencies Check
8. Repository Key Configuration
9. ROS 2 Package Repositories Sync
10. Environment Verification & Distribution Output

    
Designed by Anas Al Sami Al Harthi
