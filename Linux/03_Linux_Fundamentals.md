# 🐧 Linux Fundamentals

## Introduction

Linux Fundamentals are the core concepts required to understand and work efficiently with Linux systems. These concepts form the foundation for System Administration, DevOps, Cloud Computing, and Cybersecurity.

---

# What are Linux Fundamentals?

Linux Fundamentals include:

* Linux Architecture
* Users and Groups
* File System
* Processes
* Permissions
* Environment Variables
* Package Management
* Services and Daemons

---

# Linux Architecture Overview

```text
Applications
      ↓
Shell
      ↓
Kernel
      ↓
Hardware
```

* Applications: Programs used by users.
* Shell: Interface between user and kernel.
* Kernel: Core of the operating system.
* Hardware: Physical components of the computer.

---

# Linux Users

Linux is a multi-user operating system.

Types of users:

## 1. Root User

* Superuser of Linux.
* Has complete control over the system.
* User ID (UID): 0

Prompt:

```bash
#
```

---

## 2. Regular User

* Created for normal day-to-day tasks.
* Has limited permissions.

Prompt:

```bash
$
```

---

## 3. System User

* Used by services and applications.
* Examples:

```text
www-data
mysql
nobody
```

---

# Users Information File

Linux stores user information in:

```bash
/etc/passwd
```

View it:

```bash
cat /etc/passwd
```

---

# Groups in Linux

A group is a collection of users.

Purpose:

* Easier permission management.
* Multiple users can share resources.

View groups:

```bash
cat /etc/group
```

Check your groups:

```bash
groups
```

---

# User ID (UID)

Every user has a unique ID.

Check your UID:

```bash
id
```

Example:

```bash
uid=1000(stuti)
```

---

# Process in Linux

A process is a running program.

Examples:

* Chrome
* VS Code
* Python Program

---

# Types of Processes

## Foreground Process

Runs in the terminal.

Example:

```bash
python app.py
```

---

## Background Process

Runs in the background.

Example:

```bash
python app.py &
```

---

# View Running Processes

```bash
ps
```

Detailed view:

```bash
ps -ef
```

Real-time monitoring:

```bash
top
```

---

# Process ID (PID)

Every process has a unique Process ID.

Example:

```bash
ps -ef
```

---

# Kill a Process

```bash
kill PID
```

Force kill:

```bash
kill -9 PID
```

---

# Parent and Child Process

Every process is started by another process.

Check process tree:

```bash
pstree
```

---

# Environment Variables

Environment variables store system information and configuration settings.

Display all variables:

```bash
env
```

---

# Important Environment Variables

## HOME

Stores user's home directory.

```bash
echo $HOME
```

---

## USER

Current logged-in user.

```bash
echo $USER
```

---

## SHELL

Current shell.

```bash
echo $SHELL
```

---

## PATH

Stores executable search paths.

```bash
echo $PATH
```

---

# PATH Variable

When we execute a command:

```bash
python
ls
git
```

Linux searches for these executables inside directories mentioned in the PATH variable.

Example:

```bash
echo $PATH
```

Output:

```text
/usr/local/bin:/usr/bin:/bin
```

---

# Current Working Directory

```bash
pwd
```

---

# Current User

```bash
whoami
```

---

# Hostname

```bash
hostname
```

---

# Date and Time

```bash
date
```

---

# System Information

```bash
uname -a
```

---

# Package Management

Package Manager installs, updates, and removes software.

---

# Ubuntu/Debian

Install package:

```bash
sudo apt install package_name
```

Update packages:

```bash
sudo apt update
```

Upgrade packages:

```bash
sudo apt upgrade
```

Remove package:

```bash
sudo apt remove package_name
```

---

# CentOS/RHEL

Install package:

```bash
sudo yum install package_name
```

or

```bash
sudo dnf install package_name
```

---

# Services and Daemons

Services are background programs that continuously run.

Examples:

* SSH
* Docker
* Cron
* Nginx

---

# Check Service Status

```bash
systemctl status ssh
```

---

# Start Service

```bash
sudo systemctl start service_name
```

---

# Stop Service

```bash
sudo systemctl stop service_name
```

---

# Restart Service

```bash
sudo systemctl restart service_name
```

---

# Enable Service on Boot

```bash
sudo systemctl enable service_name
```

---

# Disable Service

```bash
sudo systemctl disable service_name
```

---

# Linux File Types

## Regular File

```text
-
```

## Directory

```text
d
```

## Symbolic Link

```text
l
```

## Block Device

```text
b
```

## Character Device

```text
c
```

---

# Multi-tasking

Linux can run multiple processes simultaneously.

Examples:

* Browser
* Terminal
* VS Code
* Docker

---

# Multi-user

Multiple users can use the same Linux machine.

---

# Why Linux Fundamentals are Important in DevOps?

DevOps engineers work daily with:

* Linux Servers
* Cloud Machines
* Containers
* Automation Scripts
* CI/CD Pipelines
* Monitoring Tools

Strong Linux fundamentals are essential for troubleshooting and automation.

---

# Interview Questions

## What is a Process?

A process is a running instance of a program.

---

## What is PID?

PID stands for Process ID.

---

## What is a Daemon?

A daemon is a background service running continuously.

---

## What is PATH?

PATH is an environment variable that stores directories where executable programs are located.

---

## Difference between Root User and Normal User?

| Root User               | Normal User                |
| ----------------------- | -------------------------- |
| UID = 0                 | UID > 0                    |
| Full access             | Limited access             |
| Can modify system files | Cannot modify system files |

---

## Difference between Foreground and Background Process?

| Foreground    | Background                |
| ------------- | ------------------------- |
| Uses terminal | Runs independently        |
| User waits    | User can continue working |

---

# Key Takeaways

✅ Linux is a multi-user operating system.

✅ Linux is a multi-tasking operating system.

✅ Every process has a PID.

✅ Environment variables store configuration information.

✅ PATH helps Linux locate commands.

✅ Services run in the background.

✅ Linux fundamentals are essential for DevOps engineers.

---

**Author:** Stuti Anand
**Repository:** Devops_learning_journey_Stuti
**Topic:** Linux Fundamentals
