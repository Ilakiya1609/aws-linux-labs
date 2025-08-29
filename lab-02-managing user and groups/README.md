#  Managing Users and Groups - Linux Lab

##  Objectives
In this lab, you will:
- Create new users with a default password  
- Create groups and assign users to the correct groups  
- Log in as different users and test permissions   

---

##  Task 1: Connect to EC2 via SSH
Connect to an **Amazon Linux EC2 instance** using the provided key pair.

### Windows Users (PuTTY)
1. Download `.ppk` key file  
2. Use **PuTTY** to connect:  

---

## Task 2: Create Users
- Create users with default password P@ssword1234!.
| First Name | Last Name | User ID   | Job Role             |
| ---------- | --------- | --------- | -------------------- |
| Alejandro  | Rosalez   | arosalez  | Sales Manager        |
| Efua       | Owusu     | eowusu    | Shipping             |
| Jane       | Doe       | jdoe      | Shipping             |
| Li         | Juan      | ljuan     | HR Manager           |
| Mary       | Major     | mmajor    | Finance Manager      |
| Mateo      | Jackson   | mjackson  | CEO                  |
| Nikki      | Wolf      | nwolf     | Sales Representative |
| Paulo      | Santos    | psantos   | Shipping             |
| Sofia      | Martinez  | smartinez | HR Specialist        |
| Saanvi     | Sarkar    | ssarkar   | Finance Specialist   |

---

## Task 3: Create Groups & Assign Users

### Create groups:

sudo groupadd Sales
sudo groupadd HR
sudo groupadd Finance
sudo groupadd Shipping
sudo groupadd Managers
sudo groupadd CEO
sudo groupadd Personnel

### Add users to groups:

| Group     | Members                        |
| --------- | ------------------------------ |
| Sales     | arosalez, nwolf                |
| HR        | ljuan, smartinez               |
| Finance   | mmajor, ssarkar                |
| Shipping  | eowusu, jdoe, psantos          |
| Managers  | arosalez, ljuan, mmajor        |
| CEO       | mjackson                       |
| Personnel | all managers + staff as needed |


---

## Task 4: Log in as Users & Test Permissions

- su - Switch User
- touch - To create a file

---

## Key Learnings

- Created users with useradd and passwd
- Created groups with groupadd and assigned users using usermod -a -G
- Verified with /etc/passwd and /etc/group
- Tested user permissions and saw how sudo attempts are logged in /var/log/secure

---

## AWS Component
- This lab used an Amazon EC2 t3.micro instance (1 vCPU, 1 GiB RAM) running Amazon Linux.

---

- Author: Ilakiya Subramani
- Completed: August 2025

---
