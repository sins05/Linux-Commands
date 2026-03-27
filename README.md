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
