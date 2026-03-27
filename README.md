# Linux Commands Cheat Sheet 🐧

A collection of essential Linux commands I use daily while learning system administration.

## File & Directory Operations

| Command | Description | Example |
|---------|-------------|---------|
| `ls -la` | List all files with details | `ls -la /home` |
| `cd` | Change directory | `cd /var/log` |
| `mkdir -p` | Create nested directories | `mkdir -p project/src` |
| `cp -r` | Copy directory recursively | `cp -r /source /backup` |
| `mv` | Move or rename | `mv old.txt new.txt` |
| `rm -rf` | Remove directory forcefully | `rm -rf /tmp/cache` |
| `find` | Search for files | `find / -name "*.conf"` |

## File Permissions

| Permission | Number | Meaning |
|-----------|--------|---------|
| rwx | 7 | Read + Write + Execute |
| rw- | 6 | Read + Write |
| r-x | 5 | Read + Execute |
| r-- | 4 | Read only |

*chmod 755 script.sh    # Owner:all, Group:read+exec, Others:read+exec
chmod 644 file.txt     # Owner:read+write, Group:read, Others:read
chown user:group file  # Change ownership*

## Networking Commands

| Command | Description |
|---------|-------------|
| `ip addr show` | Show IP addresses |
| `ping -c 4 google.com` | Test connectivity |
| `traceroute google.com` | Trace packet path |
| `netstat -tulnp` | Show listening ports |
| `ss -tulnp` | Socket statistics |
| `nslookup google.com` | DNS lookup |
| `dig google.com` | Detailed DNS query |
| `curl -I https://google.com` | HTTP headers |
| `sudo iptables -L` | List firewall rules |

## System Information

| Command | Description |
|---------|-------------|
| `uname -a` | System info |
| `df -h` | Disk usage |
| `free -h` | Memory usage |
| `top` / `htop` | Process monitor |
| `uptime` | System uptime |
| `whoami` | Current user |

## Service Management (systemd)
```bash
systemctl start nginx     # Start service
systemctl stop nginx      # Stop service
systemctl restart nginx   # Restart service
systemctl status nginx    # Check status
systemctl enable nginx    # Enable on boot
journalctl -u nginx       # View logs
```

## Package Management (Ubuntu/Debian)
```bash
sudo apt update           # Update package list
sudo apt upgrade          # Upgrade packages
sudo apt install nginx    # Install package
sudo apt remove nginx     # Remove package
```

## My Setup
- **Primary OS:** Ubuntu 22.04 LTS
- **Secondary:** Kali Linux (security tools)
- **Shell:** Bash

*Updating regularly as I learn more!*
