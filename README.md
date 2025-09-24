# Linux & DevOps Practice
# Repository documenting my hands-on Linux, Git, and DevOps learning journey.

"=== Daily Practice ==="

 "### Day 1: Learning Linux Commands and Pushing to GitHub"
 "Objective: Learn basic Linux commands, practice them, and push to GitHub."

# Linux commands practiced
pwd        # check current directory
mkdir      # create directories
cd         # navigate directories
touch      # create files
ls / la    # list files
echo "text" > file   # write text into a file
cp         # copy files
mv         # rename or move files
rm         # remove files

# Example Practice
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

# Git commands
git init
git status
git add .
git commit -m "Add Day 1 Linux command practice"
git branch -M main
git remote add origin git@github.com:alextwincy6/linux-devops-practice.git
git push -u origin main

# SSH Key Setup
ssh-keygen -t ed25519 -C "alextwincy6@gmail.com"
ssh -T git@github.com


echo "=== Day 2: File Viewing and Editing Practice ==="
echo "Objective: Learn commands to view, read, and edit files in Linux."

# Commands Practiced
echo "cat           # view file content"
echo "less          # scroll through file content (q to quit)"
echo "head -n <N>   # show the first N lines"
echo "tail -n <N>   # show the last N lines"
echo "tail -f       # follow file updates in real-time (Ctrl+C to quit)"
echo "nano          # simple terminal editor (save Ctrl+O, exit Ctrl+X)"
echo "wc            # count lines/words/bytes"
echo "|             # pipe: pass output from one command to another"

# Example Practice
mkdir -p devops_day2
cd devops_day2
nano day2_practice.txt
echo "# Linux is a powerful operating system.
# It is widely used in servers and DevOps.
# Commands practiced today: cat, less, head, tail, nano, wc, pipes (|)" > day2_practice.txt

# Viewing file
cat day2_practice.txt
less day2_practice.txt
head -n 5 day2_practice.txt
tail -n 5 day2_practice.txt

# Follow updates live
tail -f day2_practice.txt

# Count lines, words, bytes
wc day2_practice.txt
cat day2_practice.txt | wc -l

echo "Notes:"
echo "- Each folder contains notes.txt, tasks.txt, and scripts for that day."
echo "- README will be updated daily as learning progresses."
