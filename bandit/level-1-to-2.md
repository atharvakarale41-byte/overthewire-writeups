# Bandit Level 1 → Level 2

## Level Goal

The password for the next level is stored in a file called `-` located in the home directory.

## Commands You May Need

`ls`, `cd`, `cat`, `file`, `du`, `find`

## Solution

### Step 1: Log in with SSH

Log in using the previous Bandit password:

```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
```

### Step 2: List the files

```bash
ls -al
```

You will notice a file named `-`.

### Step 3: Read the file correctly

Because the filename is just a hyphen, you must reference it explicitly:

```bash
cat ./-
```

The output is the password for **Bandit Level 2**. It is intentionally not included here.
