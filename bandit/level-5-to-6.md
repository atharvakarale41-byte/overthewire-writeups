# Bandit Level 5 → Level 6

## Level Goal

The password for the next level is stored in a file somewhere under the `inhere` directory and has all of the following properties:

- human-readable
- 1033 bytes in size
- not executable

## Commands You May Need

`ls`, `cd`, `cat`, `file`, `du`, `find`

## Solution

### Step 1: Log in with SSH

Log in using the previous Bandit password:

```bash
ssh bandit5@bandit.labs.overthewire.org -p 2220
```

### Step 2: List the directory contents

```bash
ls
```

### Step 3: Enter the `inhere` directory

```bash
cd inhere
ls
```

You will see many subdirectories.

### Step 4: Search for the file with the correct properties

```bash
find . -type f -size 1033c ! -executable
```

This will return the exact file path.

Example result:

```bash
./maybehere07/.file2
```

### Step 5: Read the file

```bash
cat ./maybehere07/.file2
```

The output is the password for **Bandit Level 6**. It is intentionally not included here.
