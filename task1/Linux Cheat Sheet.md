# Linux Cheat Sheet

## File & Directory Operations
- `ls` - List directory contents
- `ls -la` - Detailed list including hidden files
- `cd` - Change directory
- `pwd` - Print working directory
- `mkdir` - Create directory
- `rm -rf` - Recursive and forced removal
- `cp` - Copy files
- `mv` - Move/Rename files
- `cat` - Concatenate/View files
- `nano` / `vi` / `vim` - Text editors

## System Information
- `uname -a` - System info
- `hostname` - Network name
- `whoami` - Current user
- `id` - User and group IDs
- `uptime` - How long the system has been running
- `free -m` - Memory usage
- `df -h` - Disk space usage

## Network Utilities
- `ifconfig` / `ip addr` - Interface details
- `ping` - Check connectivity
- `netstat -tulnp` - Active ports and services
- `ss -antp` - Socket statistics
- `dig` / `nslookup` - DNS lookup
- `curl` - Transfer data from/to a server
- `wget` - Download files from the web

## Permissions & Ownership
- `chmod [permissions] [file]` - Change permissions
- `chown [user]:[group] [file]` - Change ownership
- `sudo` - Execute command as superuser

## Process Management
- `ps aux` - List all processes
- `top` / `htop` - Interactive process viewer
- `kill -9 [PID]` - Force stop a process

## Package Management (Debian/Kali)
- `apt update` - Update repository index
- `apt upgrade` - Upgrade all packages
- `apt install [package]` - Install software
- `apt remove [package]` - Uninstall software
