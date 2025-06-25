# Daily Linux Administrator Learning Plan (Hour-by-Hour Breakdown):

## Phase 1: The Absolute Basics (Weeks 1):
- **Goal**: Get comfortable with the command line interface (CLI) and basic navigation.


# Week 1: Getting Started

## Day 1: Introduction to Linux & VM Setup (1 hour)
- What is Linux? Why is it used for servers?
- Introduction to different distributions (Ubuntu, CentOS/RHEL, Debian).
- Action: Download VirtualBox/VMware Player and an Ubuntu Server ISO. Begin the installation process for your first VM.

## Day 2: First Login & Basic Commands (1 hour)
- Complete VM setup.
- Login to your Linux VM.
- ls (list files/directories), pwd (print working directory), cd (change directory).
- Understanding absolute vs. relative paths.

## Day 3: File & Directory Management I (1 hour)
- mkdir (make directory), rmdir (remove empty directory).
- touch (create empty file).
- cp (copy files/directories).

## Day 4: File & Directory Management II (1 hour)
- mv (move/rename files/directories).
- rm (remove files/directories - be careful with this one!).
- cat (concatenate and display file content), less (view file content page by page).

## Day 5: Permissions Basics (1 hour)
- Understanding ls -l output (permissions, owner, group, size, date).
- chmod (change permissions - focus on octal notation for now, e.g., chmod 755 file).

## Day 6: User & Group Management I (1 hour)
- What are users and groups?
- whoami, id.
- sudo (executing commands as root - very important!).

## Day 7: Review & Practice (1 hour)
- Go back through all commands learned.
- Create a complex directory structure with files, copy, move, rename, and delete them.
- Change permissions on various files.


### Week 2: More Core Utilities

## Day 8: User & Group Management II (1 hour)
- useradd (add user), passwd (set user password).
- userdel (delete user).
- groupadd, groupdel.
- usermod (modify user accounts).
## Day 9: Text Editors (1 hour)
- Learn a basic text editor: nano is highly recommended for beginners.
- Practice creating, editing, and saving files.
- (Optional: Briefly look at vi/vim - acknowledge its existence, but don't dive deep yet unless curious).
## Day 10: Process Management I (1 hour)
- What are processes?
- ps (display running processes).
- top (monitor processes dynamically).
- kill (terminate processes).
## Day 11: Disk Usage & File Search (1 hour)
- df (display free disk space).
- du (estimate file space usage).
- find (search for files/directories).
## Day 12: Archiving & Compression (1 hour)
- tar (archive files).
- gzip, gunzip, bzip2, bunzip2 (compression).
- Combining tar with compression (e.g., tar -czvf).
## Day 13: Package Management Basics (1 hour)
- Understand what package managers are (APT for Debian/Ubuntu, YUM/DNF for RedHat/CentOS).
- sudo apt update, sudo apt upgrade (Ubuntu/Debian).
- sudo apt install <package>, sudo apt remove <package>.
- (If using CentOS: sudo yum update, sudo yum install <package>).
## Day 14: Review & Simple Scripting (1 hour)
- Review all commands from Week 2.
- Write your first very simple shell script (e.g., a script that prints "Hello, Linux!").
- Make it executable (chmod +x script.sh) and run it.
