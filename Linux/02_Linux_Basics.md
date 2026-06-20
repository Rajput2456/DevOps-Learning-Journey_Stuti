# 🐧 Linux Basics

## Introduction

Linux is a free and open-source operating system based on Unix. It was created by **Linus Torvalds** in 1991 and is widely used in servers, cloud computing, cybersecurity, and DevOps.

Most modern servers, cloud platforms, and DevOps tools run on Linux.

---

# What is an Operating System?

An Operating System (OS) is software that acts as an interface between the user and computer hardware.

### Responsibilities of an Operating System

* Managing CPU
* Managing Memory (RAM)
* Managing Files and Directories
* Managing Hardware Devices
* Running Applications
* Providing Security

Examples:

* Linux
* Windows
* macOS

---

# What is Linux?

Linux is:

* Open Source
* Multi-user Operating System
* Multi-tasking Operating System
* Secure
* Stable
* Highly Customizable

---

# Why Linux is Popular in DevOps?

## 1. Open Source

Linux is free to use and modify.

## 2. Stability

Linux servers can run continuously for months or years.

## 3. Security

Linux provides strong security and permission management.

## 4. Automation Friendly

Most DevOps tools work efficiently on Linux.

## 5. Cloud Compatibility

Cloud platforms like AWS, Azure, and GCP primarily use Linux servers.

---

# Linux Distributions (Distros)

A Linux Distribution is a complete operating system built using the Linux Kernel.

Popular Linux distributions:

* Ubuntu
* Debian
* CentOS
* Red Hat Enterprise Linux (RHEL)
* Fedora
* Kali Linux
* Arch Linux

---

# Linux Architecture

```text
+----------------------+
|     Applications     |
+----------------------+
|         Shell        |
+----------------------+
|        Kernel        |
+----------------------+
|      Hardware        |
+----------------------+
```

---

# Hardware

Physical components of the computer.

Examples:

* CPU
* RAM
* Hard Disk
* Keyboard
* Mouse
* Network Card

---

# Kernel

The Kernel is the heart of the Linux Operating System.

It acts as a bridge between software and hardware.

It is Written in C Language

### Responsibilities of Kernel

* Process Management
* Memory Management
* Device Management
* File System Management
* Security Management

---

# Shell

The Shell is a command interpreter.

It accepts commands from the user and sends them to the kernel.

It Control  the Kernel

Examples:

* Bash
* Zsh
* Sh
* Ksh

---

# Terminal

The Terminal is an application used to interact with the shell.

Examples:

* Ubuntu Terminal
* Windows Terminal
* PowerShell
* GNOME Terminal

---

# Linux Boot Process

The Linux boot process consists of:

### Step 1: BIOS/UEFI

Performs hardware initialization.

### Step 2: Bootloader

Loads the operating system.

Example:

```
GRUB
```

### Step 3: Kernel Loading

Loads the Linux kernel into memory.

### Step 4: Init/Systemd

Starts system services.

### Step 5: User Login

User can log in and start working.

---

# Linux File System

Linux follows a hierarchical file system structure.

Everything in Linux is treated as a file.

---

# Important Linux Directories

## /

Root directory. This is the top-most directory.

## /home

Contains users' personal files.

Example:

```bash
/home/stuti
```

## /root

Home directory of the root user.

## /etc

Contains configuration files.

Examples:

```bash
/etc/passwd
/etc/hosts
/etc/ssh
```

## /bin

Contains essential user commands.

Examples:

```bash
ls
cp
mv
cat
```

## /sbin

Contains system administration commands.

Examples:

```bash
reboot
shutdown
fdisk
```

## /usr

Contains user applications and programs.

## /var

Contains variable data.

Examples:

* Logs
* Cache
* Mail

## /tmp

Stores temporary files.

## /dev

Contains device files.

Examples:

```bash
/dev/sda
/dev/null
```

## /proc

Contains information about running processes and the kernel.

---

# Linux Users

Linux supports multiple users.

Examples:

* Root User
* Normal User
* Service User

---

# Root User

The root user has complete control over the system.

Prompt:

```bash
#
```

---

# Normal User

Regular users with limited permissions.

Prompt:

```bash
$
```

---

# Multi-user Operating System

Multiple users can use the system simultaneously.

---

# Multi-tasking Operating System

Linux can run multiple programs at the same time.

Examples:

* Browser
* Terminal
* VS Code

---

# Case Sensitivity

Linux is case-sensitive.

Example:

```bash
file.txt
File.txt
FILE.txt
```

All are different files.

---

# Absolute Path

Path starting from the root directory.

Example:

```bash
/home/stuti/project
```

---

# Relative Path

Path relative to the current directory.

Example:

```bash
project/file.txt
```

---

# Hidden Files

Files beginning with a dot (`.`) are hidden.

Examples:

```bash
.git
.bashrc
.profile
```

To view hidden files:

```bash
ls -la
```

---

# Command Syntax

```bash
command [options] [arguments]
```

Example:

```bash
ls -la /home
```

* ls → command
* -la → option
* /home → argument

---

# Linux Package Managers

Different distributions use different package managers.

### Ubuntu/Debian

```bash
apt
```

### RHEL/CentOS

```bash
yum
dnf
```

---

# Basic System Information Commands

Check current user:

```bash
whoami
```

Check current directory:

```bash
pwd
```

Check operating system:

```bash
uname -a
```

Check hostname:

```bash
hostname
```

Check current date:

```bash
date
```

Check calendar:

```bash
cal
```

---

# Why Linux is Important for DevOps Engineers?

A DevOps Engineer uses Linux for:

* Server Administration
* Automation
* Shell Scripting
* Docker
* Kubernetes
* CI/CD Pipelines
* Cloud Computing
* Monitoring and Troubleshooting

---

# Interview Questions

### What is Linux?

Linux is an open-source Unix-like operating system.

### What is Kernel?

Kernel is the core component of Linux that manages hardware and system resources.

### What is Shell?

Shell is a command interpreter that allows users to communicate with the operating system.

### Difference Between Terminal and Shell?

| Terminal           | Shell               |
| ------------------ | ------------------- |
| Application        | Command Interpreter |
| Provides Interface | Executes Commands   |

### Why is Linux used in DevOps?

Because it is stable, secure, open-source, and most servers and cloud platforms run on Linux.

---

# Key Takeaways

✅ Linux is an open-source operating system.

✅ Linux uses a hierarchical file system.

✅ Everything in Linux is treated as a file.

✅ Linux is multi-user and multi-tasking.

✅ The Kernel is the heart of Linux.

✅ The Shell allows users to interact with the operating system.

✅ Linux is the foundation of most DevOps tools and cloud platforms.

---


