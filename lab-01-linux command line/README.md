# Linux Command Line Lab  

## Objectives  
In this lab, you will:  
- Run commands to gain knowledge of your current system and session  
- Search and run previous bash commands  

---


## Task1: Run Familiar Commands  

### Identify User and System Information  

whoami        # Display current username
hostname -s   # Show short hostname
uptime -p     # Show system uptime in readable format
who -H -a     # Show logged-in users and details
TZ=America/New_York date
TZ=America/Los_Angeles date
cal -j   # Calendar with Julian dates
cal -s   # Calendar starting on Sunday
cal -m   # Calendar starting on Monday
id ec2-user  # Show UID, GID, and group info

---

## Task2: Improve Workflow with History and Search

history
date   # Show current date
!!     # Re-run the last command

---

## Key Learnings

whoami, hostname, and uptime → system basics
who -H -a → see active users and session details
TZ=<region> date → check time in different locations
cal -j, cal -s, cal -m → work with calendars
id <user> → check UID/GID/group memberships
history, CTRL+R, !! → improve workflow and save time

---

## About the AWS Component
- This lab used an Amazon EC2 t3.micro instance (1 vCPU, 1 GiB RAM) running Amazon Linux.

--- 
Author: Ilakiya Subramani
Completed: July 2025
