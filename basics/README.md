````markdown
# Shell Basic Commands

This repository contains simple shell scripts, each demonstrating one basic command or concept in the Linux shell.

Each file is an executable script that performs exactly one action, corresponding to the tasks listed below.

Repository root: `/root/holbertonschool-shell`  
Project folder: `basics/`

---

## Tasks & Scripts

### Task 0: Print current working directory
**Script:** `basics/0-current_working_directory`  
Prints the absolute path of the current working directory.

Command used:
```bash
pwd
````

---

### Task 1: Display contents of current directory

**Script:** `basics/1-listit`
Lists the files and directories in the current directory.

Command used:

```bash
ls
```

---

### Task 2: Go to the user’s home directory

**Script:** `basics/2-bring_me_home`
Changes the working directory to the user’s home directory.

Command used:

```bash
cd
```

---

### Task 3: List in long format

**Script:** `basics/3-listfiles`
Displays the contents of the current directory in long (detailed) format.

Command used:

```bash
ls -l
```

---

### Task 4: List all, including hidden files (long format)

**Script:** `basics/4-listmorefiles`
Shows all files (including hidden ones starting with `.`) in long format.

Command used:

```bash
ls -la
```

---

### Task 5: List with numeric user and group IDs

**Script:** `basics/5-listfilesdigitonly`
Shows all files (including hidden) in long format, displaying the user and group IDs numerically.

Command used:

```bash
ls -na
```

---

### Task 6: Create a directory

**Script:** `basics/6-firstdirectory`
Creates a directory called `MyFirstDirectory` under `/tmp`.

Command used:

```bash
mkdir /tmp/MyFirstDirectory
```

---

### Task 7: Move a file into the directory

**Script:** `basics/7-movethatfile`
Moves the file `betty` into `/tmp/MyFirstDirectory`.

Command used:

```bash
mv /tmp/betty /tmp/MyFirstDirectory
```

---

### Task 8: Delete a file

**Script:** `basics/8-firstdelete`
Removes the file `betty` from `/tmp/MyFirstDirectory`.

Command used:

```bash
rm /tmp/MyFirstDirectory/betty
```

---

### Task 9: Delete a directory

**Script:** `basics/9-firstdirdeletion`
Removes the directory `/tmp/MyFirstDirectory`.

Command used:

```bash
rmdir /tmp/MyFirstDirectory
```

---

### Task 10: Change to the previous directory

**Script:** `basics/10-back`
Switches back to the previous working directory.

Command used:

```bash
cd -
```

---

### Task 11: List multiple directories (including hidden, long format)

**Script:** `basics/11-lists`
Lists, in long format, all files (including hidden) in:

* the current directory (`.`)
* the parent directory (`..`)
* the `/boot` directory

Command used:

```bash
ls -al . .. /boot
```

---

### Task 12: Print the type of a file

**Script:** `basics/12-file_type`
Displays the type of the file `/tmp/iamafile`.

Command used:

```bash
file /tmp/iamafile
```

---

### Task 13: Create a symbolic link

**Script:** `basics/13-symbolic_link`
Creates a symbolic link named `ls` that points to `/bin/ls` in the current directory.

Command used:

```bash
ln -s /bin/ls ls
```

---

### Task 14: Copy HTML files to the parent directory

**Script:** `basics/14-copy_html`
Copies all files with the `.html` extension from the current directory to its parent directory.

Command used:

```bash
cp *.html ..
```

---

### Task 15: Move files with uppercase names

**Script:** `basics/15-lets_move`
Moves all files whose names start with an uppercase letter into the `/tmp/u` directory.

Command used:

```bash
mv [[:upper:]]* /tmp/u
```

---

### Task 16: Delete backup files

**Script:** `basics/16-clean_emacs`
Deletes all files in the current directory whose names end with a tilde (`~`), typically backup files.

Command used:

```bash
rm *~
```

---

### Task 17: Create a nested directory structure

**Script:** `basics/17-tree`
Creates the directory tree `welcome/to/school` in the current directory, including any missing parent directories.

Command used:

```bash
mkdir -p welcome/to/school
```

---

## Usage

From the repository root:

1. Make scripts executable (if not already):

   ```bash
   chmod u+x basics/*
   ```

2. Run a script, for example:

   ```bash
   ./basics/0-current_working_directory
   ```

Each script is designed to demonstrate a single command in a clear and simple way.

```
