# Basic Linux Commands

This document contains commonly used Linux commands for beginners, DevOps learners, and system administrators.

---

## 1. pwd

**Purpose:** Display the current working directory.

```bash
pwd
```

Example Output:

```bash
/home/stuti
```

---

## 2. ls

**Purpose:** List files and directories.

```bash
ls
```

---

## 3. ls -la

**Purpose:** List all files, including hidden files, with detailed information.

```bash
ls -la
```

---

## 4. cd

**Purpose:** Change directory.

```bash
cd Documents
```

Move back one directory:

```bash
cd ..
```

Go to home directory:

```bash
cd ~
```

---

## 5. mkdir

**Purpose:** Create a new directory.

```bash
mkdir project
```

---

## 6. rmdir

**Purpose:** Remove an empty directory.

```bash
rmdir project
```

---

## 7. touch

**Purpose:** Create an empty file.

```bash
touch file.txt
```

---

## 8. cat

**Purpose:** Display file contents.

```bash
cat file.txt
```

---

## 9. nano

**Purpose:** Edit files using Nano editor.

```bash
nano file.txt
```

Save: `Ctrl + O`

Exit: `Ctrl + X`

---

## 10. cp

**Purpose:** Copy files and directories.

Copy a file:

```bash
cp file.txt backup.txt
```

Copy a directory:

```bash
cp -r folder1 folder2
```

---

## 11. mv

**Purpose:** Move or rename files.

Rename a file:

```bash
mv old.txt new.txt
```

Move a file:

```bash
mv file.txt Documents/
```

---

## 12. rm

**Purpose:** Remove files and directories.

Delete a file:

```bash
rm file.txt
```

Delete a Non-empty directory:

```bash
rm -r folder
```

Force delete: Permanent Delete

```bash
rm -rf folder
```

Delete Empty Files :

```bash
rmdir folder
```

---

## 13. clear

**Purpose:** Clear terminal screen.

```bash
clear
```

---

## 14. echo

**Purpose:** Print text or write content into files.

Print text:

```bash
echo "Hello Linux"
```

Write text to file:

```bash
echo "Hello Linux" > file.txt
```

Append text to file:

```bash
echo "New Line" >> file.txt
```

---

## 15. grep

**Purpose:** Search text within files.

```bash
grep "hello" file.txt
```

---

## 16. find

**Purpose:** Search for files and directories.

```bash
find . -name "file.txt"
```

---

## 17. chmod

**Purpose:** Change file permissions.

```bash
chmod 755 script.sh
```

Make file executable:

```bash
chmod +x script.sh
```

---

## 18. chown

**Purpose:** Change file ownership.

```bash
sudo chown user:user file.txt
```

---

## 19. df -h

**Purpose:** Display disk usage.

```bash
df -h
```

---

## 20. free -h

**Purpose:** Display memory usage.

```bash
free -h
```

---

## 21. top

**Purpose:** Monitor running processes.

```bash
top
```

Press `q` to quit.

---

## 22. ps

**Purpose:** Show active processes.

```bash
ps aux
```

---

## 23. kill

**Purpose:** Terminate a process.

```bash
kill PID
```

Force terminate:

```bash
kill -9 PID
```

---

## 24. uname

**Purpose:** Display system information.

```bash
uname -a
```

---

## 25. whoami

**Purpose:** Display the current user.

```bash
whoami
```

---

## 26. history

**Purpose:** Show previously executed commands.

```bash
history
```

---

## 27. wget

**Purpose:** Download files from the internet.

```bash
wget https://example.com/file.zip
```

---

## 28. curl

**Purpose:** Transfer data from URLs.

```bash
curl https://example.com
```

---

## 29. ping

**Purpose:** Check network connectivity.

```bash
ping google.com
```

---

## 30. ssh

**Purpose:** Connect to a remote server securely.

```bash
ssh username@server-ip
```

---

## 31. scp

**Purpose:** Securely copy files between systems.

```bash
scp file.txt user@server:/home/user/
```

---

## 32. zip

**Purpose:** Compress files and folders.

```bash
zip -r project.zip project/
```

---

## 33. unzip

**Purpose:** Extract ZIP archives.

```bash
unzip project.zip
```

---

## 34. tar

**Purpose:** Create and extract archive files.

Create archive:

```bash
tar -cvf backup.tar folder/
```

Extract archive:

```bash
tar -xvf backup.tar
```

---

## 35. man

**Purpose:** Display command manual.

```bash
man ls
```

---
## 36. sudo

**Purpose:** Execute commands with administrative privilege

```bash
sudo apt update
---

# Conclusion

These Linux commands are essential for:
- Linux Administration
- DevOps Engineering
- Cloud Computing
- System Management
- Git and GitHub Workflows
- Server Management

Mastering these commands will help build a strong foundation in Linux and DevOps.

