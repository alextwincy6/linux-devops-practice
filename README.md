# Day 2: File Viewing and Editing Practice

**Objective:** Learn commands to view, read, and edit files in Linux.

## Commands Practiced
- `cat` – view file content
- `less` – scroll through long files (`q` to quit)
- `head -n <N>` – show the first N lines
- `tail -n <N>` – show the last N lines
- `tail -f` – follow file updates in real time (`Ctrl+C` to quit)
- `nano` – terminal editor (save with `Ctrl+O`, exit `Ctrl+X`)
- `wc` – count lines/words/bytes (`wc -l`, `wc -w`)


---

## 📄 Example Practice

```bash
# Create folder for Day 2
mkdir -p devops_day2
cd devops_day2

# Create a practice file
nano day2_practice.txt
# Add content about Linux commands and practice notes
# Example content:
# Linux is a powerful operating system.
# It is widely used in servers and DevOps.
# Commands practiced today: cat, less, head, tail, nano, wc, pipes (|)

# Save and exit (Ctrl+O, Enter, Ctrl+X)

# View file content
cat day2_practice.txt
less day2_practice.txt
head -n 5 day2_practice.txt
tail -n 5 day2_practice.txt

# Follow updates live
tail -f day2_practice.txt

# Count lines, words, and bytes
wc day2_practice.txt
cat day2_practice.txt | wc -l
