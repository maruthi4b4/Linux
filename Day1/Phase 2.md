# Phase 2: Networking & System Administration Fundamentals (Weeks 3-4)

**Goal : understand basic networking, system services, and a deeper dive into administrative tasks.**

## Week 3: Networking & Services

## Day 15: Network Configuration Basics (1 hour)
- ip addr (display IP addresses).
- ping (test network connectivity).
- netstat (network statistics - though ss is more modern).
- ss (socket statistics).

## Day 16: DNS & SSH (1 hour)
- nslookup or dig (DNS lookups).
- What is SSH? Why is it important for administrators?
- Basic ssh connection from your host OS to your VM.

## Day 17: Managing Services (systemd) (1 hour)
- Introduction to systemd (the modern init system).
- sudo systemctl status <service>, sudo systemctl start <service>, sudo systemctl stop <service>, sudo systemctl enable <service>, sudo systemctl disable <service>.
- Practice with services like sshd or apache2 (if installed).

## Day 18: Log Files (1 hour)
- Where are logs stored? (/var/log).
- tail -f (follow log files in real-time).
- grep (search within files, especially logs).

## Day 19: Scheduling Tasks (cron) (1 hour)
- What is cron?
- crontab -e (edit user's crontab).
- Understand cron syntax (minutes, hours, day of month, month, day of week, command).
- Schedule a simple task (e.g., write "hello" to a file every minute).

## Day 20: Software Installation & Compilation (1 hour)
- Beyond package managers: how to install from source (conceptual understanding).
- wget or curl (download files from the internet).
- Basic steps: ./configure, make, sudo make install (don't do this often on production servers, but understand the concept).

## Day 21: Review & Advanced grep / find (1 hour)
- Review networking commands and service management.
- Practice more complex grep patterns (regular expressions).
- Practice find with actions (e.g., find . -name "*.txt" -delete).

## Week 4: Advanced Administration Concepts

## Day 22: Disk Partitioning & Filesystems (Conceptual) (1 hour)
- What are partitions? Filesystems (ext4, XFS).
- lsblk (list block devices).
- mount, umount (mounting filesystems).
- Briefly introduce /etc/fstab (persistent mounts).

## Day 23: Logical Volume Management (LVM) - Conceptual (1 hour)
- Why use LVM? (Flexibility, resizing).
- Understand Physical Volumes (PVs), Volume Groups (VGs), Logical Volumes (LVs).
- (Hands-on LVM might take more than an hour, but understand the theory).

## Day 24: SSH Key-Based Authentication (1 hour)
- More secure than passwords.
- ssh-keygen (generate keys).
- ssh-copy-id (copy public key to server).
- Practice logging in without a password.

## Day 25: Basic Firewall (UFW/firewalld) (1 hour)
- Why firewalls are important.
- Ubuntu/Debian: ufw status, ufw enable, ufw allow ssh, ufw deny http.
- CentOS/RHEL: sudo systemctl status firewalld, sudo firewall-cmd --add-service=ssh --permanent, sudo firewall-cmd --reload.

## Day 26: Backups & Restores (Conceptual + Simple Script) (1 hour)
- Importance of backups.
- Simple backup strategy using tar and rsync (conceptual).
- Write a simple script to backup a directory to another location on the VM.

## Day 27: Introduction to Shell Scripting (Deeper Dive) (1 hour)
- Variables, if statements, for loops.
- Write a script that takes arguments and performs a simple task.

## Day 28: Project Day / Troubleshooting (1 hour)
- Choose a small project: e.g., set up a basic web server (Apache/Nginx) on your VM, enable its service, allow it through the firewall, and access it from your host.
- Intentionally break something and try to fix it using your learned skills (e.g., delete a critical file, try to restore or troubleshoot).

- ## Going Forward (After the First Month):
- **Automation**: Ansible, Puppet, Chef.
- **Virtualization**: Deeper into KVM, Docker, Kubernetes.
- **Cloud**: AWS, Azure, GCP.
- **Monitoring**: Nagios, Zabbix, Prometheus.
- **Specific Services**: Web servers (Apache, Nginx), databases (MySQL, PostgreSQL), mail servers.
- **Security**: SELinux/AppArmor, advanced firewalling, intrusion detection.
- **Advanced Scripting**: More complex shell scripts, Python for administration.
