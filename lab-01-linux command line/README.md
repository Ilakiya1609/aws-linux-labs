# Linux Command Line Lab  

## Objectives  
In this lab, you will:  
- Run commands to gain knowledge of your current system and session  
- Search and run previous bash commands  

---


## Task1: Run Familiar Commands  

### Identify User and System Information  

1. whoami        # Display current username
2. hostname -s   # Show short hostname
3. uptime -p     # Show system uptime in readable format
4. who -H -a     # Show logged-in users and details
5. TZ=America/New_York date
6. TZ=America/Los_Angeles date
7. cal -j   # Calendar with Julian dates
8. cal -s   # Calendar starting on Sunday
9. cal -m   # Calendar starting on Monday
10. id ec2-user  # Show UID, GID, and group info

---

## Task2: Improve Workflow with History and Search

1. history
2. date   # Show current date
3. !!     # Re-run the last command

---

## Key Learnings

1. whoami, hostname, and uptime → system basics
2. who -H -a → see active users and session details
3. TZ=<region> date → check time in different locations
4. cal -j, cal -s, cal -m → work with calendars
5. id <user> → check UID/GID/group memberships
6. history, CTRL+R, !! → improve workflow and save time

---

## About the AWS Component
- This lab used an Amazon EC2 t3.micro instance (1 vCPU, 1 GiB RAM) running Amazon Linux.

--- 
- Author: Ilakiya Subramani
- Completed: July 2025
