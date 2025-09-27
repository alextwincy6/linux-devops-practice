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
- touch file1.txt
- ls -l file1.txt

### Step 2: Change file permissions
- chmod 700 file1.txt
- chmod 654 file1.txt

### Step 3: Check file permissions
- ls -l file1.txt

### Step 4: Change ownership
- sudo chown alex_injeti file1.txt
- sudo chown alex_injeti:test_group file1.txt

### Step 5: Change group only
- sudo chgrp test_group file1.txt

### Step 6: Verify owner and group
- ls -l file1.txt
- groups alex_injeti

### Notes:
- `r` = read, `w` = write, `x` = execute
- File permissions format: owner | group | others
- Groups allow multiple users to share access

## Day 4: Text Processing Essentials

** Objective: Learn and practice Linux text processing commands like grep, cut, sort, uniq, wc, tr, head, tail.

## 📂 Commands Practiced

- grep <pattern> <file> – search for a pattern in a file

- cut -d<delimiter> -f<fields> <file> – extract specific columns

- sort <file> – sort lines alphabetically

- uniq -c <file> – count unique lines (use with sort)

- wc <file> – count lines, words, and bytes

- tr <set1> <set2> – translate or delete characters

- head -n <N> – show the first N lines

- tail -n <N> – show the last N lines

## 📄 Example Practice
# Step 1: Create a sample file
mkdir -p day4_practice/linux_day4
cd day4_practice/linux_day4
echo -e "apple\nbanana\napple\norange\nbanana\napple" > fruits.txt

# Step 2: Count unique fruits
cat fruits.txt | sort | uniq -c

# Step 3: Filter fruits containing 'a'
grep 'a' fruits.txt

# Step 4: Extract first column using cut (example)
cut -d' ' -f1 fruits.txt

# Step 5: Get first 2 lines
head -n 2 fruits.txt

# Step 6: Get last 2 lines
tail -n 2 fruits.txt

# Step 7: Count lines, words, characters
wc fruits.txt

# Step 8: Replace lowercase 'a' with '@'
tr 'a' '@' < fruits.txt
## 📌 Notes

Pipes | allow chaining commands: cat fruits.txt | sort | uniq -c

grep is case-sensitive by default; use -i for case-insensitive search

Combine sort and uniq -c to count repeated items

Always practice with small sample files before applying commands to real data
