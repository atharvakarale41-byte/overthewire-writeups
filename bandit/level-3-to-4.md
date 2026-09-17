# Bandit Level 3 → Level 4

## Level Goal

The password for the next level is stored in a hidden file somewhere in the `inhere` directory.

## Commands You May Need

`ls`, `cd`, `cat`, `file`, `du`, `find`

## Solution

### Step 1: Log in with SSH

Log in using the previous Bandit password:

```bash
ssh bandit3@bandit.labs.overthewire.org -p 2220
```

### Step 2: Go to the `inhere` directory and list hidden files

```bash
cd inhere
ls -la
```

You will see a hidden file in the directory.

### Step 3: Read the hidden file

```bash
cat .hidden
```

The output is the password for **Bandit Level 4**. It is intentionally not included here.
