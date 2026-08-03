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
