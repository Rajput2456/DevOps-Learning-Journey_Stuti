# 📁 File and Directory Management in Linux

## Introduction

Everything in Linux is stored as a file. Managing files and directories is one of the most important skills for Linux administrators and DevOps engineers.

This document covers creating, deleting, copying, moving, and searching files and directories.

---

# Why File Management is Important?

* Organize project files
* Store logs and configuration files
* Manage application data
* Automate system administration tasks
* Work efficiently on Linux servers

---

# Understanding Files and Directories

* **File:** Stores data.
* **Directory (Folder):** Stores files and other directories.

Example:

```text
/home/stuti/project
│
├── app.py
├── README.md
└── logs
```

---

# Check Current Directory

```bash
pwd
```

Example:

```bash
/home/stuti/project
```

---

# List Files and Directories

```bash
ls
```

---

# Detailed Listing

```bash
ls -l
```

---

# Show Hidden Files

```bash
ls -la
```

---

# Change Directory

```bash
cd directory_name
```

Example:

```bash
cd project
```

---

# Move One Directory Back

```bash
cd ..
```

---

# Go to Home Directory

```bash
cd
```

or

```bash
cd ~
```

---

# Create a Directory

```bash
mkdir project
```

---

# Create Multiple Directories

```bash
mkdir dir1 dir2 dir3
```

---

# Create Nested Directories

```bash
mkdir -p project/src/python
```

---

# Remove Empty Directory

```bash
rmdir directory_name
```

---

# Remove Directory Recursively

```bash
rm -r directory_name
```

---

# Force Delete Directory

```bash
rm -rf directory_name
```

⚠️ Be careful with `rm -rf`.

---

# Create File

```bash
touch file.txt
```

---

# Create Multiple Files

```bash
touch file1.txt file2.txt file3.txt
```

---

# Copy File

```bash
cp source destination
```

Example:

```bash
cp file1.txt backup.txt
```

---

# Copy Directory

```bash
cp -r project backup_project
```

---

# Move File

```bash
mv file.txt Documents/
```

---

# Rename File

```bash
mv old.txt new.txt
```

---

# Delete File

```bash
rm file.txt
```

---

# Search Files

```bash
find . -name "*.txt"
```

---

# Search Directory

```bash
find . -type d
```

---

# Search Files Only

```bash
find . -type f
```

---

# Display Directory Structure

```bash
tree
```

Install:

```bash
sudo apt install tree
```

---

# Display File Type

```bash
file filename
```

Example:

```bash
file app.py
```

---

# Count Files

```bash
ls | wc -l
```

---

# Create Hidden File

```bash
touch .env
```

---

# Create Hidden Directory

```bash
mkdir .config
```

---

# Wildcards

## All Files

```bash
*
```

Example:

```bash
ls *
```

---

## Specific Extension

```bash
*.txt
```

---

## Single Character

```bash
?
```

Example:

```bash
ls file?.txt
```

---

# Absolute Path

Starts from root.

```bash
/home/stuti/project
```

---

# Relative Path

Starts from current directory.

```bash
project/app.py
```

---

# Command Summary

| Command | Purpose                  |
| ------- | ------------------------ |
| pwd     | Current directory        |
| ls      | List files               |
| ls -la  | Show hidden files        |
| cd      | Change directory         |
| mkdir   | Create directory         |
| rmdir   | Remove empty directory   |
| touch   | Create file              |
| cp      | Copy files               |
| mv      | Move/Rename              |
| rm      | Delete files             |
| find    | Search files             |
| tree    | Show directory structure |
| file    | Show file type           |

---

# Hands-on Practice

## Task 1

Create directory structure:

```bash
mkdir -p DevOps/Linux/Notes
```

---

## Task 2

Create files:

```bash
touch file1.txt file2.txt
```

---

## Task 3

Copy file:

```bash
cp file1.txt backup.txt
```

---

## Task 4

Rename file:

```bash
mv file2.txt notes.txt
```

---

## Task 5

Delete file:

```bash
rm backup.txt
```

---

# Mini Project

Create this structure:

```text
DevOps_Project
│
├── Scripts
├── Notes
├── Logs
└── README.md
```

Commands:

```bash
mkdir Scripts Notes Logs
touch README.md
tree
```

---

# Interview Questions

### Difference between `cp` and `mv`?

* `cp` copies files.
* `mv` moves or renames files.

---

### Difference between `rm -r` and `rm -rf`?

* `rm -r` removes recursively.
* `rm -rf` removes recursively and forcefully.

---

### What is a hidden file?

A file starting with `.`.

Example:

```bash
.gitignore
.env
```

---

### Difference between Absolute and Relative Path?

Absolute path starts from `/`.

Relative path starts from the current directory.

---

# Key Takeaways

✅ Linux stores everything as files.

✅ `mkdir` creates directories.

✅ `touch` creates files.

✅ `cp` copies files.

✅ `mv` moves and renames files.

✅ `rm` deletes files.

✅ `find` searches files.

✅ `tree` displays directory structure.

---

