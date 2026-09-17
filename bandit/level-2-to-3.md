# Bandit Level 2 → Level 3

## Level Goal

The password for the next level is stored in a hidden file in the `inhere` directory.

## Commands You May Need

`ls`, `cd`, `cat`, `file`, `du`, `find`

## Solution

### Step 1: Log in with SSH

Log in using the previous Bandit password:

```bash
ssh bandit2@bandit.labs.overthewire.org -p 2220
```

### Step 2: Enter the `inhere` directory and list hidden files

```bash
cd inhere
ls -a
```

The listing includes the hidden file `...Hiding-From-You`.

### Step 3: Read the hidden file

```bash
cat ./...Hiding-From-You
```

The output is the password for **Bandit Level 3**. It is intentionally not included here.
