# Bandit Level 4 → Level 5

## Level Goal

The password for the next level is stored in the only human-readable file in the `inhere` directory.

Tip: if your terminal is messed up, try the `reset` command.

## Commands You May Need

`ls`, `cd`, `cat`, `file`, `du`, `find`

## Solution

### Step 1: Log in with SSH

Log in using the previous Bandit password:

```bash
ssh bandit4@bandit.labs.overthewire.org -p 2220
```

### Step 2: Go to the `inhere` directory and inspect the files

```bash
ls
cd inhere
ls -l
```

You will find several files, each with different types.

### Step 3: Find the human-readable file

Use `file` to check each file or inspect them one by one:

```bash
file ./*
```

The only file that is human-readable is the correct one.

### Step 4: Read the correct file

```bash
cat ./-file07
```

The output is the password for **Bandit Level 5**. It is intentionally not included here.
