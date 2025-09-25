<<<<<<< HEAD
# linux-devops-practice
 “Linux for DevOps learning journey”.
=======
# Linux & DevOps Practice
This repository documents my hands-on Linux, Git, and DevOps learning journey, tracking each day’s exercises and practice.

---

## Daily Practice

### Day 1: Learning Linux Commands and Pushing to GitHub
**Objective:** Learn basic Linux commands, practice them with examples, and push the learning to GitHub.

#### Commands Practiced
- `pwd` – check current directory
- `mkdir` – create directories
- `cd` – navigate between directories
- `touch` – create files
- `ls` / `la` – list files
- `echo "text" > file` – write text into a file
- `cp` – copy files
- `mv` – rename or move files
- `rm` – remove files

#### Example Practice

# Create a folder for Day 1
mkdir devops_day1
cd devops_day1

# Create files
touch notes.txt tasks.txt

# Add content to notes
echo "Hello, this is my first Linux command practice" > notes.txt

# Copy notes
cp notes.txt notes_backup.txt

# Rename tasks file
mv tasks.txt todo.txt

# Remove a file
rm old_file.txt

# Linux & DevOps Practice - Day 2
This folder documents my Day 2 hands-on learning for Linux file viewing and editing commands.

---

## Daily Practice

### Day 2: File Viewing and Editing Practice
**Objective:** Learn and practice commands to view, read, and edit files in Linux.

#### Commands Practiced
- `cat` – view file content
- `less` – scroll through file content (q to quit)
- `head -n <N>` – show the first N lines
- `tail -n <N>` – show the last N lines
- `tail -f` – follow file updates in real-time (Ctrl+C to quit)
- `nano` – simple terminal editor (save Ctrl+O, exit Ctrl+X)
- `wc` – count lines/words/bytes
- `|` (pipe) – pass output from one command to another

#### Example
# Create a folder and file for Day 2
- mkdir -p devops_day2
- cd devops_day2
- nano day2_practice.txt

# Add content about Linux commands and practice notes
 - "Linux is a powerful operating system.
- It is widely used in servers and DevOps.
- Commands practiced today: cat, less, head, tail, nano, wc, pipes (|)" > day2_practice.txt

# Viewing and inspecting file
- cat day2_practice.txt
- less day2_practice.txt
- head -n 5 day2_practice.txt
- tail -n 5 day2_practice.txt

# Follow updates live
- tail -f day2_practice.txt

# Count lines, words, bytes
- wc day2_practice.txt
- cat day2_practice.txt | wc -l


## Day 3: File Permissions, Ownership, and Groups
### Objective:
Learn Linux file permissions, ownership, and groups commands.

### Step 1: Create a file
touch file1.txt
ls -l file1.txt

### Step 2: Change file permissions
chmod 700 file1.txt
chmod 654 file1.txt

### Step 3: Check file permissions
ls -l file1.txt

### Step 4: Change ownership
sudo chown alex_injeti file1.txt
sudo chown alex_injeti:test_group file1.txt

### Step 5: Change group only
sudo chgrp test_group file1.txt

### Step 6: Verify owner and group
ls -l file1.txt
groups alex_injeti

### Notes:
- `r` = read, `w` = write, `x` = execute
- File permissions format: owner | group | others
- Groups allow multiple users to share access
