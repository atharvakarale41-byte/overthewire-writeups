# Bandit Level 1 → Level 2

## Level Goal

The password for the next level is stored in a file called `--spaces in this filename--` located in the home directory.

## Commands You May Need

`ls`, `cd`, `cat`, `file`, `du`, `find`

## Helpful Reading Material

- Google Search for “spaces in filename”

## Solution

### Step 1: Log in with SSH

Log in using the previous Bandit password:

```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
```

### Step 2: List the files

```bash
ls
```

You will find the file named `--spaces in this filename--`.

### Step 3: Read the file

Because the filename begins with hyphens and contains spaces, use a relative path and escape the spaces:

```bash
cat ./--spaces\ in\ this\ filename--
```

The output is the password for **Bandit Level 2**. It is intentionally not included here.
