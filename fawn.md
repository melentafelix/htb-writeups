
# Hack The Box: Fawn

## Overview
Fawn is a Starting Point machine focused on FTP and anonymous login.

## Steps

### 1. Scan the target
nmap -sV <target-ip>

Port 21 was open, running vsftpd 3.0.3.

### 2. Connect over FTP
ftp <target-ip>

Logged in with the username `anonymous` and no password.
Server responded with `230 Login successful`.

### 3. Find and download the flag
ls
get flag.txt
exit

### 4. Read the flag
cat flag.txt

Flag: [redacted]

## What I learned
- FTP sends data in cleartext, so it is insecure.
- Anonymous login can expose files to anyone.
- SFTP (over SSH) is the secure alternative.
