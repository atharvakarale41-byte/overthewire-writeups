# Bandit Level 0 → Level 1

## Goal

Log in to the Bandit game using the credentials provided on the OverTheWire website, then find the password for the next level.

## Connection

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

When prompted, enter the Level 0 password from the official OverTheWire instructions.

## Solution

After logging in, list the files in the home directory:

```bash
ls
```

The directory contains a file named `readme`. Read it with:

```bash
cat readme
```

The output is the password for **Bandit Level 1**. It is intentionally not included here.

## Key Command

```bash
cat readme
```

## Notes

- The SSH service uses port `2220`, not the default SSH port `22`.
- Passwords are redacted from this write-up repository.
