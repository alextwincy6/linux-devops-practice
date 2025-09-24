# Linux & DevOps Practice

This repository documents my hands-on learning journey for Linux and Git, tracking each day’s exercises and practice.

---

## Daily Practice

### Day 1: Learning Linux Commands and Pushing to GitHub

**Objective:** Learn basic Linux commands, practice them with examples, and push the learning to GitHub.

---

### 1️⃣ Linux Commands Learned and Practiced

I practiced the following commands in Ubuntu/WSL:

- `pwd` – to check the current directory
- `mkdir` – to create directories
- `cd` – to navigate between directories
- `touch` – to create files
- `ls` / `la` – to list files
- `echo "text" > file` – to write text into a file
- `cp` – to copy files
- `mv` – to rename or move files
- `rm` – to remove files

**Examples I practiced:**

```bash
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

#After praticing Linux commands , I pushed my learning to GitHub:

# Initialize Git repository
git init

# Check status
git status

# Add all files
git add .

# Commit changes
git commit -m "Add Day 1 Linux command practice"

# Rename branch to main
git branch -M main

# Add remote repository (SSH)
git remote add origin git@github.com:alextwincy6/linux-devops-practice.git

# Push changes to GitHub
git push -u origin main


#SSH Key Setup (for secure GitHub access):

ssh-keygen -t ed25519 -C "alextwincy6@gmail.com"
ssh -T git@github.com

#After this, I successfully pushed all my Day 1 practice to GitHub.
## Notes

## Day 2: File Viewing and Editing Practice

**Objective:** Learn commands to view and edit files in Linux.

##Commands Practiced:

cat – view file content

less – scroll through file content

head – view first lines

tail – view last lines

nano – edit files in terminal

wc – count lines, words, bytes

Pipes | – combine commands

Example Practice:

# Create a folder for Day 2
mkdir devops_day2
cd devops_day2

# Create a practice file
nano day2_practice.txt

# Add content about Linux commands and practice notes
# Example content:
# Linux is a powerful operating system.
# It is widely used in servers and DevOps.
# Commands practiced today: cat, less, head, tail, nano, wc, pipes (|)

# Save and exit (Ctrl+O, Enter, Ctrl+X)

Check and view file content:

cat day2_practice.txt
less day2_practice.txt
head day2_practice.txt
tail day2_practice.txt
tail -f day2_practice.txt  # real-time monitoring
wc day2_practice.txt        # line/word/byte count
cat day2_practice.txt | wc -l  # count lines via pipe

- Each folder contains `notes.txt`, `tasks.txt`, and scripts for that day.
- This README will be updated as I continue learning.
