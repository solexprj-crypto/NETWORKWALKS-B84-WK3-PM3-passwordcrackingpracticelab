# NETWORKWALKS-B84-WK3-PM3-passwordcrackingpracticelab
Password cracking practice lab

Password Cracking Lab - Encrypted PDF

Objective
Crack the password of an encrypted PDF document using John the Ripper in a controlled lab environment.

Tools Used
- Kali Linux
- John the Ripper / Johnny (GUI)
- pdf2john
- rockyou.txt wordlist

Methodology

1. Extract Hash from PDF
```bash
pdf2john encrypted.pdf > pdf_hash.txt
 2. Crack Hash with John
john --wordlist=/usr/share/wordlists/rockyou.txt pdf_hash.txt
 3. Show Cracked Password
john --show pdf_hash.txt
 Result
 Password successfully recovered

## Lesson Learned
Weak passwords in common wordlists can be cracked in seconds. Always use long, unique passphrases and enable MFA.

 Disclaimer
This lab was performed in a controlled environment for educational purposes only.
.
