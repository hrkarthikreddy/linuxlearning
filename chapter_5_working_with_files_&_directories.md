# Chapter 5: Working with Files and Directories

## 🗂️ Overview

In Linux, everything is represented as a file—including hardware devices, directories, and processes. Mastering file and directory management is essential for any Linux user or administrator. This chapter walks you through navigating the filesystem, creating, copying, moving, deleting, and linking files and directories, and using various tools to manage them efficiently.

---

## 🗃️ Filesystem Structure and Hierarchy

Linux uses a hierarchical directory structure:

```plaintext
/
├── bin/        # Essential user binaries
├── boot/       # Boot loader files
├── dev/        # Device files
├── etc/        # Configuration files
├── home/       # User home directories
├── lib/        # Essential shared libraries
├── tmp/        # Temporary files
├── usr/        # Secondary hierarchy for read-only user data
└── var/        # Variable data like logs and databases
```

### Example:
```bash
cd /usr/bin
ls -lh
```

---

## 🧭 Navigating the Filesystem

### Commands:

- `pwd`: Displays the current directory.
- `cd <path>`: Changes directory.
- `ls`: Lists directory contents.

### Special Characters:

- `.`: Current directory
- `..`: Parent directory
- `~`: Home directory

### Examples:
```bash
cd /etc
pwd  # Outputs: /etc
cd ~  # Go to home directory
cd -  # Return to the previous directory
```

---

## 📄 Creating and Viewing Files

### Creating:
- `touch file.txt`: Create an empty file
- `echo "text" > file.txt`: Write content to a new file

### Viewing:
- `cat file.txt`: Display full content
- `less file.txt`: Scrollable view
- `head -n 5 file.txt`: First 5 lines
- `tail -n 5 file.txt`: Last 5 lines
- `tail -f logfile`: Live output from a log file

### Example:
```bash
echo "Welcome to Linux" > welcome.txt
cat welcome.txt
```

---

## 🔁 Copying, Moving, and Deleting Files

### Commands:

- `cp file1 file2`: Copy
- `mv file1 newloc/`: Move or rename
- `rm file1`: Delete file
- `rm -r folder/`: Delete directory recursively

### Example:
```bash
mkdir test
cd test
touch file1.txt file2.txt
cp file1.txt copy_file1.txt
mv file2.txt renamed_file2.txt
rm copy_file1.txt
```

---

## 📌 File and Directory Permissions

### Permissions Explained:

```plaintext
-rwxr-xr--  1 user group 123 Jan 01 10:00 file.sh
```

- `r` = read (4)
- `w` = write (2)
- `x` = execute (1)

### Commands:
- `chmod 755 script.sh`: Sets executable permissions
- `chown user:group file`: Changes ownership

### Examples:
```bash
chmod +x script.sh
chown john:john config.cfg
```

---

## 🧷 Creating Links

### Hard vs Symbolic Links:

- **Hard Link**: Reference to the same inode
- **Symbolic Link (Symlink)**: A pointer to another file

### Commands:
- `ln file1 file2`: Hard link
- `ln -s file1 symlink`: Symlink

### Example:
```bash
touch original.txt
ln original.txt hardlink.txt
ln -s original.txt symlink.txt
```

---

## 🔍 Finding Files and Commands

### Commands:
- `find / -name "file.txt"`
- `locate file.txt`
- `which bash`
- `whereis bash`

### Example:
```bash
find /home -type f -name "notes.txt"
which python3
```

---

## 🗃 Directory Management

### Commands:
- `mkdir newdir`: Create directory
- `rmdir olddir`: Remove empty directory
- `rm -r dir`: Remove non-empty directory

### Example:
```bash
mkdir -p projects/linux/scripts
cd projects/linux
ls
```

---

## 🧠 Mind Map (Suggested)

```plaintext
[Working with Files and Directories]
       ├── Navigating Filesystem (cd, pwd, ls)
       ├── Creating and Viewing Files (touch, cat, less)
       ├── File Operations (cp, mv, rm)
       ├── Permissions (chmod, chown)
       ├── Linking Files (ln, ln -s)
       └── Finding Tools (find, locate)
```

---

## 📚 References

- https://www.geeksforgeeks.org/linux-file-system/
- https://linuxize.com/post/understanding-linux-file-permissions/
- https://www.tutorialspoint.com/unix/unix-file-management.htm
- https://www.redhat.com/sysadmin/basic-linux-commands

---

