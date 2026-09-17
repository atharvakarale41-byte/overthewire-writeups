# Bandit Level 2 → Level 3

## Level Goal

The password for the next level is stored in a file called `spaces in this filename`.

## Commands You May Need

`ls`, `cd`, `cat`, `file`, `du`, `find`

## Solution

### Step 1: Log in with SSH

Log in using the previous Bandit password:

```bash
ssh bandit2@bandit.labs.overthewire.org -p 2220
```

### Step 2: List the files in the home directory

```bash
ls
```

You will find a file named `spaces in this filename`.

### Step 3: Read the file correctly

Because the filename contains spaces, escape them with backslashes:

```bash
cat ./spaces\ in\ this\ filename
```

The output is the password for **Bandit Level 3**. It is intentionally not included here.
