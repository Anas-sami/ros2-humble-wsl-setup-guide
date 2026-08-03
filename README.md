# ros2-humble-wsl-setup-guide
A comprehensive guide and visual documentation for installing and configuring ROS 2 Humble on Windows using WSL 2. Created for Smart Methods  (AI Track ).

# 🚀 ROS 2 Humble Setup Guide on Windows using WSL2

<p align="center">

![ROS2](https://img.shields.io/badge/ROS-2-22314E?style=for-the-badge)
![Ubuntu](https://img.shields.io/badge/Ubuntu-22.04-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![Windows](https://img.shields.io/badge/Windows-11-0078D4?style=for-the-badge&logo=windows)
![WSL2](https://img.shields.io/badge/WSL2-Linux-4EAA25?style=for-the-badge&logo=linux&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-success?style=for-the-badge)

</p>

---

## 📖 Overview

This repository provides a complete guide to installing **ROS 2 Humble Hawksbill** on **Windows 11** using **Windows Subsystem for Linux 2 (WSL2)**.

The project documents the complete installation journey, including system preparation, Ubuntu installation, package management, repository configuration, dependency troubleshooting, and solutions to common installation issues.

Unlike many tutorials that only demonstrate the successful outcome, this repository also documents real installation errors and explains how to resolve them.

---

# ✨ Features

- Complete WSL2 installation
- Ubuntu 22.04 installation
- Windows PowerShell setup
- ROS 2 repository configuration
- Linux package management
- Dependency troubleshooting
- Broken package recovery
- Environment configuration
- Real installation screenshots
- Beginner-friendly documentation

---

# 🛠 Technologies

- Windows 11
- Windows Subsystem for Linux (WSL2)
- Ubuntu 22.04 LTS
- ROS 2 Humble
- Bash
- PowerShell
- APT Package Manager
- Linux Terminal

---

# 📂 Repository Structure

```text
.
├── README.md
└── png for linux
    ├── gid1.png
    ├── gid2.png
    ├── gid3.png
    ├── gid5.png
    ├── gid6.png
    ├── gid7.png
    ├── gid8.png
    ├── gid9.png
    └── gid10.png
```

---

# 🚀 Installation Process

## Step 1 — Enable WSL2

Enable the required Windows features.

- Virtual Machine Platform
- Windows Subsystem for Linux

These components provide the virtualization environment required to run Linux on Windows.

<p align="center">
<img src="png%20for%20linux/gid1.png" width="900">
</p>

---

## Step 2 — Install Windows Subsystem for Linux

Windows automatically installs the WSL infrastructure before downloading Ubuntu.

<p align="center">
<img src="png%20for%20linux/gid2.png" width="900">
</p>

---

## Step 3 — Install Ubuntu

Ubuntu is downloaded and installed using the WSL installer.

After installation, Ubuntu becomes the primary Linux environment used for ROS 2 development.

<p align="center">
<img src="png%20for%20linux/gid10.png" width="900">
</p>

---

## Step 4 — Install Ubuntu from PowerShell

Run the following command:

```powershell
wsl --install -d Ubuntu-22.04
```

<p align="center">
<img src="png%20for%20linux/gid3.png" width="900">
</p>

---

## Step 5 — Update Ubuntu

Before installing ROS 2, update your operating system.

```bash
sudo apt update
sudo apt upgrade
```

Updating packages helps prevent dependency conflicts.

<p align="center">
<img src="png%20for%20linux/gid9.png" width="900">
</p>

---

## Step 6 — Install Required Dependencies

Install the packages required before configuring the ROS repositories.

```bash
sudo apt install software-properties-common curl
```

<p align="center">
<img src="png%20for%20linux/gid7.png" width="900">
</p>

---

## Step 7 — Configure the ROS 2 Repository

Add the official ROS repository and refresh the package list.

```bash
sudo apt update
```

<p align="center">
<img src="png%20for%20linux/gid8.png" width="900">
</p>

---

# ⚠ Troubleshooting

One objective of this repository is documenting common installation problems and their solutions.

---

## Broken Packages

Package conflicts may occur because of:

- Incorrect Ubuntu version
- Interrupted installation
- Missing dependencies
- Repository mismatch
- Outdated package cache

<p align="center">
<img src="png%20for%20linux/gid5.png" width="900">
</p>

---

## Missing setup.bash

If you receive the following error:

```text
/opt/ros/humble/setup.bash: No such file or directory
```

This usually indicates that ROS 2 has not been installed successfully.

Verify the installation before sourcing the environment.

<p align="center">
<img src="png%20for%20linux/gid6.png" width="900">
</p>

---

# 📚 What You Will Learn

By following this guide, you will learn how to:

- Install WSL2
- Install Ubuntu on Windows
- Configure Linux
- Manage packages using APT
- Configure ROS repositories
- Install ROS 2 Humble
- Troubleshoot installation errors
- Resolve dependency issues
- Configure the ROS environment
- Prepare a robotics development workspace

---

# 🎯 Target Audience

This project is intended for:

- Robotics Students
- Software Engineering Students
- Computer Science Students
- Linux Beginners
- ROS Beginners
- Robotics Developers
- AI Engineers
- Embedded Systems Engineers

---

# 💡 Why This Repository?

Most installation tutorials only show the successful installation process.

This repository documents the real installation experience, including common errors, troubleshooting procedures, and practical solutions, helping others build a reliable ROS 2 development environment with confidence.

---

# 📸 Installation Gallery

## Enable WSL2

<img src="png%20for%20linux/gid1.png">

---

## Install WSL

<img src="png%20for%20linux/gid2.png">

---

## PowerShell Installation

<img src="png%20for%20linux/gid3.png">

---

## Ubuntu Installation

<img src="png%20for%20linux/gid10.png">

---

## Install Dependencies

<img src="png%20for%20linux/gid7.png">

---

## Update Packages

<img src="png%20for%20linux/gid9.png">

---

## Configure Repository

<img src="png%20for%20linux/gid8.png">

---

## Broken Packages

<img src="png%20for%20linux/gid5.png">

---

## Missing setup.bash

<img src="png%20for%20linux/gid6.png">

---

# 👤 Author

**Anas Sami Alharthi**

---

# 📄 License

This project is licensed under the MIT License.
