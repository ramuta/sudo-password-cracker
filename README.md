# sudo-password-cracker (spcracker.py)

Python script that helps you crack the password of the current unix shell user.

## Requirements

- Python 3 (could also work on Python 2, but haven't tested it)

## Usage

Let's say you gained access to a Linux server and have a shell as some user. You don't know what the sudo password of 
this user is, but you'd like to brute force it.

Instead of manually typing `sudo -i` and trying out different passwords, you can use this Python script to automate the 
process:

    python spcracker.py rockyou.txt

As you can see, you need to provide the script a wordlist with possible passwords (one password per line). One of the 
best password wordlists is `rockyou.txt`.

> Please, do not use this script for illegal activities. It's for ethical pentesting purposes only.

## Known issues

The script may return a false positive in a form of a password starting with a `#` or `#1`. If you have an idea how to 
solve it, please open an issue or submit a PR. Thanks! :)

## TODO:

- Figure out a solution for the `#` false positives
