# HTB - Meow (Starting Point)

## Machine Info
- Name: Meow
- Difficulty: Very Easy
- OS: Linux

## Recon
- Ran nmap scan against target
- Found port 23/tcp open running telnet

## Exploitation
- Connected to target via telnet:
  telnet <TARGET_IP>
- Logged in as `root` with a blank password (no password required)

## Post-Exploitation
- Already in root's home directory upon login
- Located flag.txt and read its contents using `cat flag.txt`

## Flag
- Root flag: [REDACTED]

## Lessons Learned
- Telnet is an insecure, unencrypted protocol and should not be used for remote administration
- Default/blank credentials are a critical misconfiguration
