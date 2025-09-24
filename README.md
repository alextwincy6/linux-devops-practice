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

---

### **Day 2: File Viewing and Editing Practice**

**Objective:** Learn and practice commands to view, read, and edit files in the terminal.

#### 📂 Commands Practiced
- `cat` – view file content  
- `less` – view long files page-by-page (`q` to quit)  
- `head -n <N>` – show the first N lines  
- `tail -n <N>` – show the last N lines  
- `tail -f` – follow file updates in real time (quit with `Ctrl+C`)  
- `nano` – simple terminal editor (save with `Ctrl+O`, exit `Ctrl+X`)  
- `wc` – count lines/words/bytes (`wc -l`, `wc -w`)  
- `|` (pipe) – pass output from one command to another

#### 📄 Example Practice (run these in a terminal)
```bash
# create folder and file
mkdir -p devops_day2
cd devops_day2
nano day2_practice.txt    # paste/enter the sample content, save & exit

# view and inspect
cat day2_practice.txt
less day2_practice.txt
head -n 5 day2_practice.txt
tail -n 5 day2_practice.txt

# follow updates live (open two terminals to test)
tail -f day2_practice.txt

# counts
wc day2_practice.txt
cat day2_practice.txt | wc -l



- Each folder contains `notes.txt`, `tasks.txt`, and scripts for that day.
- This README will be updated as I continue learning.
