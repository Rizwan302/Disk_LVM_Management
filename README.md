📦 Ansible LVM Automation Role


A fully automated Ansible Role for creating, managing, extending, and removing Logical Volumes (LVM) using variables and dictionary-based configuration.

This project is designed as part of a professional-level Linux & Automation learning program and is suitable for real enterprise use.

🚀 Project Overview

This Ansible role automates complete LVM lifecycle operations:

Create Physical Volumes (PV)

Create Volume Groups (VG)

Create Multiple Logical Volumes (LV) using dictionary variables

Format filesystems (ext4, xfs)

Mount filesystems persistently

Extend logical volumes

Remove LV, VG, PV

Wipe filesystem signatures

📁 Role Folder Structure
roles/lvm/
│── tasks/
│    ├── main.yml
│    ├── create.yml
│    ├── extend.yml
│    ├── remove.yml
│
│── handlers/
│    └── main.yml
│
│── defaults/
│    └── main.yml
│
│── vars/
│    └── main.yml
│
│── README.md

🧩 Features Included (Labs 18 → 23)
✅  Create LV & Mount Persistently

Create VG (vg_logs)

Create LVs (lv_old_logs, lv_new_logs)

Format LV (ext4 / xfs)

Mount on:


✅ Remove LV and Wipe FS

Unmount both LVs

Remove LVs

Remove VG

Remove PV on /dev/sdb and /dev/sdc

Wipe filesystem signatures

✅ Extend Existing LV

Extend lv_old_logs by +500M

Resize ext4 filesystem

✅ Complete Role Implementation

This role uses:

Handlers for formatting & mounting automatically

Tasks for PV, VG, LV creation

Loops for multiple LVs

Notifications for modular automation

3️⃣ Run the Role

🛠️ Technologies Used
Technology	    Purpose
Ansible	        Automation engine
LVM2	        Volume management
YAML	        Configuration files
Linux           RHEL / CentOS / Oracle Linux


🏆 Why This Project Is Resume-Ready

✔ Hands-on Linux storage automation
✔ Real-world production-level role
✔ Modular, scalable, clean YAML code
✔ Implements notifications, handlers, loops, variables, best practices
✔ Shows DevOps skills: Ansible + LVM + Linux filesystem
