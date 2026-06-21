# 🔐 Linux File Permissions and Ownership

## 📌 Introduction

Linux is a multi-user operating system. To provide security, Linux uses a permission system that controls who can read, write, or execute files and directories.

Every file and directory in Linux has:

- Owner (User)
- Group
- Permissions

Permissions help protect data and prevent unauthorized access to the system.

---

# Why File Permissions are Important?

Permissions are used to:

- Protect sensitive files
- Restrict unauthorized access
- Secure system resources
- Control user activities
- Improve system security

---

# Understanding Linux Permissions

Run:

```bash
ls -l
```

Example Output:

```bash
-rwxr-xr-- 1 stuti stuti 500 Jun 18 file.txt
```

Breakdown:

```text
-rwxr-xr--
│ │ │ │
│ │ │ └── Others
│ │ └──── Group
│ └────── Owner
└──────── File Type
```

---

# File Types

| Symbol | Meaning |
|--------|----------|
| - | Regular File |
| d | Directory |
| l | Symbolic Link |
| c | Character Device |
| b | Block Device |

Examples:

```bash
-rw-r--r-- file.txt
drwxr-xr-x project
```

---

# Permission Types

| Permission | Symbol | Value |
|------------|---------|--------|
| Read | r | 4 |
| Write | w | 2 |
| Execute | x | 1 |

---

# Permission Groups

```text
rwx rwx rwx
│   │   │
│   │   └── Others
│   └────── Group
└────────── Owner
```

---

# Read Permission (r)

Allows user to:

- View file contents
- List directory contents

Example:

```bash
cat file.txt
```

---

# Write Permission (w)

Allows user to:

- Modify file contents
- Delete files
- Create files inside directories

---

# Execute Permission (x)

Allows user to:

- Run scripts
- Execute programs
- Enter directories

---

# Viewing Permissions

```bash
ls -l
```

Example:

```bash
-rw-r--r-- file.txt
```

---

# Changing Permissions using chmod

## Syntax

```bash
chmod permissions filename
```

Example:

```bash
chmod 755 script.sh
```

---

# Symbolic Method

## Add Permission

```bash
chmod u+x script.sh
```

---

## Remove Permission

```bash
chmod g-w script.sh
```

---

## Give Read Permission to Others

```bash
chmod o+r script.sh
```

---

# Symbols Used in chmod

| Symbol | Meaning |
|---------|----------|
| u | User (Owner) |
| g | Group |
| o | Others |
| a | All |

Examples:

```bash
chmod u+x file.sh
chmod g+w file.sh
chmod o-r file.sh
chmod a+x file.sh
```

---

# Numeric Method

Permission Values:

```text
Read    = 4
Write   = 2
Execute = 1
```

---

# Common Permission Values

| Number | Permission |
|---------|------------|
| 777 | rwxrwxrwx |
| 755 | rwxr-xr-x |
| 744 | rwxr--r-- |
| 700 | rwx------ |
| 644 | rw-r--r-- |
| 600 | rw------- |

---

# Examples

## Full Permission

```bash
chmod 777 file.txt
```

---

## Owner Full Access

```bash
chmod 700 file.txt
```

---

## Common File Permission

```bash
chmod 644 file.txt
```

---

## Common Script Permission

```bash
chmod 755 script.sh
```

---

# Changing Ownership using chown

## Syntax

```bash
sudo chown user filename
```

Example:

```bash
sudo chown stuti file.txt
```

---

# Change User and Group

```bash
sudo chown stuti:developers file.txt
```

---

# Changing Group using chgrp

```bash
sudo chgrp developers file.txt
```

---

# Recursive Permission Changes

## Change Permissions Recursively

```bash
chmod -R 755 project
```

---

## Change Ownership Recursively

```bash
sudo chown -R stuti:developers project
```

---

# Special Permissions

## SUID (Set User ID)

```bash
chmod u+s file
```

When a user runs the file, it executes with the owner's permissions.

---

## SGID (Set Group ID)

```bash
chmod g+s directory
```

Files created inside the directory inherit the directory's group.

---

## Sticky Bit

```bash
chmod +t directory
```

Example:

```bash
chmod 1777 /tmp
```

Prevents users from deleting files owned by others.

---

# User Information Commands

## Check Current User

```bash
whoami
```

---

## Check User ID

```bash
id
```

---

## Check User Groups

```bash
groups
```

---

# Practical Example

Create a script:

```bash
touch script.sh
```

Give execute permission:

```bash
chmod +x script.sh
```

Verify:

```bash
ls -l
```

Run:

```bash
./script.sh
```

---

# Mini Project

## Step 1: Create Directory

```bash
mkdir DevOps_Project
cd DevOps_Project
```

---

## Step 2: Create Script

```bash
touch deploy.sh
```

---

## Step 3: Give Execute Permission

```bash
chmod 755 deploy.sh
```

---

## Step 4: Verify Permissions

```bash
ls -l
```

---

## Step 5: Change Owner

```bash
sudo chown username deploy.sh
```

---

# Interview Questions

### 1. What is chmod?

Used to change file permissions.

---

### 2. What is chown?

Used to change file ownership.

---

### 3. What is the difference between 755 and 777?

| Permission | Meaning |
|------------|----------|
| 755 | Owner has full access, others can read and execute |
| 777 | Everyone has full access |

---

### 4. What is SUID?

Allows a file to run with the owner's privileges.

---

### 5. What is Sticky Bit?

Prevents users from deleting files owned by other users.

---

# Frequently Used Commands Cheat Sheet

```bash
ls -l
chmod 755 file
chmod +x script.sh
chmod -R 755 folder
chown user file
chown user:group file
chgrp group file
whoami
id
groups
```

---

# Hands-on Practice Tasks

### Task 1

Create a file and give execute permission.

### Task 2

Create a directory and assign 755 permission.

### Task 3

Change file ownership.

### Task 4

Apply recursive permissions to a directory.

### Task 5

Create a shared directory using SGID.

---

# Key Takeaways

✅ Linux uses permissions to secure files and directories.

✅ Every file has an owner and a group.

✅ `chmod` changes permissions.

✅ `chown` changes ownership.

✅ `chgrp` changes group ownership.

✅ `755` and `644` are the most commonly used permissions in DevOps.

---

