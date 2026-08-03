# ros2-humble-wsl-setup-guide
A comprehensive guide and visual documentation for installing and configuring ROS 2 Humble on Windows using WSL 2. Created for Smart Methods  (AI Track ).

# 🚀 ROS 2 Humble on WSL2 (Windows 11)

<p align="center">

![ROS2](https://img.shields.io/badge/ROS-2-blue?style=for-the-badge)
![Ubuntu](https://img.shields.io/badge/Ubuntu-22.04-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![WSL2](https://img.shields.io/badge/WSL2-Windows_11-0078D4?style=for-the-badge&logo=windows)
![Linux](https://img.shields.io/badge/Linux-Ubuntu-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-success?style=for-the-badge)

</p>

---

# 📖 Overview

This repository documents the complete process of installing **ROS 2 Humble Hawksbill** on **Windows 11** using **Windows Subsystem for Linux 2 (WSL2)**.

Instead of showing only the successful installation, this project also documents common installation problems, package dependency issues, repository configuration, troubleshooting techniques, and practical solutions encountered during the setup process.

The repository is intended to help robotics students, software engineers, AI developers, and Linux beginners install ROS 2 with confidence while understanding every step of the workflow.

---

# ✨ Features

- Complete WSL2 installation
- Ubuntu installation on Windows
- ROS 2 repository configuration
- Linux environment setup
- Package management using APT
- Dependency troubleshooting
- Broken package recovery
- Terminal command documentation
- Real installation screenshots
- Beginner-friendly workflow

---

# 🛠 Technologies

- Windows 11
- Windows Subsystem for Linux (WSL2)
- Ubuntu 22.04 LTS
- ROS 2 Humble Hawksbill
- PowerShell
- Bash
- APT Package Manager
- Linux Terminal

---

# 📂 Repository Structure

```
.
├── README.md
└── PNG for Linux
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

# 🚀 Installation Workflow

## Step 1 — Install WSL2

Enable the required Windows components:

- Virtual Machine Platform
- Windows Subsystem for Linux

These components provide the virtualization layer required to run Ubuntu on Windows.

<p align="center">
<img src="PNG%20for%20Linux/gid1.png" width="900">
</p>

---

## Step 2 — Install Windows Subsystem for Linux

Windows installs WSL automatically before downloading Ubuntu.

<p align="center">
<img src="PNG%20for%20Linux/gid2.png" width="900">
</p>

---

## Step 3 — Install Ubuntu

Ubuntu is downloaded and installed through the WSL installer.

This Linux environment will host ROS 2 and all robotics development tools.

<p align="center">
<img src="PNG%20for%20Linux/gid10.png" width="900">
</p>

---

## Step 4 — Launch Ubuntu from PowerShell

Install Ubuntu directly using PowerShell.

```powershell
wsl --install -d Ubuntu-22.04
```

<p align="center">
<img src="PNG%20for%20Linux/gid3.png" width="900">
</p>

---

## Step 5 — Update Ubuntu

Update the operating system before installing ROS 2.

```bash
sudo apt update
sudo apt upgrade
```

Updating packages helps avoid dependency conflicts during installation.

<p align="center">
<img src="PNG%20for%20Linux/gid9.png" width="900">
</p>

---

## Step 6 — Install Required Dependencies

Install the packages required by ROS repositories.

Example:

```bash
sudo apt install software-properties-common curl
```

<p align="center">
<img src="PNG%20for%20Linux/gid7.png" width="900">
</p>

---

## Step 7 — Configure the ROS Repository

Add the official ROS repository and refresh the package list.

```bash
sudo apt update
```

<p align="center">
<img src="PNG%20for%20Linux/gid8.png" width="900">
</p>

---

# ⚠ Troubleshooting

Real installation problems are documented throughout this project.

Understanding these issues is just as important as completing the installation.

---

## Broken Packages

Dependency conflicts can occur when:

- Incorrect Ubuntu version
- Interrupted installation
- Outdated repositories
- Missing dependencies
- Repository mismatch

<p align="center">
<img src="PNG%20for%20Linux/gid5.png" width="900">
</p>

---

## Missing setup.bash

If you receive:

```text
/opt/ros/humble/setup.bash: No such file or directory
```

it usually means ROS 2 was not installed successfully.

Verify the installation before sourcing the environment.

<p align="center">
<img src="PNG%20for%20Linux/gid6.png" width="900">
</p>

---

# 📚 What You Will Learn

After completing this guide you will understand how to:

- Install WSL2
- Install Ubuntu
- Configure Linux on Windows
- Manage Linux packages
- Configure ROS repositories
- Install ROS 2 Humble
- Solve dependency issues
- Recover from broken packages
- Configure the ROS environment
- Build a robotics development workspace

---

# 🎯 Target Audience

- Robotics Students
- Software Engineering Students
- Computer Science Students
- Linux Beginners
- ROS Beginners
- AI Engineers
- Robotics Developers
- Embedded Systems Engineers

---

# 💡 Why This Repository?

Most installation tutorials only demonstrate the ideal installation process.

This repository documents the complete journey, including real-world errors, troubleshooting techniques, and practical solutions, making it easier for others to reproduce a successful ROS 2 installation on Windows using WSL2.

---

# 👤 Author

**Anas Sami Alharthi**

---

# 📄 License

This project is licensed under the MIT License.
