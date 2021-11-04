# Good to know commands
Show disk space - Only see ext4 file system:
```bash
df -h -t ext4
```
Find all files larger than 10 Megabytes:
```bash
find / -size +10M -ls
```
Delete Cardano pool logs older than 1 day
```bash
find /opt/cardano/cnode/logs/archive/ -mtime +1 -name "*.json" -print -exec /bin/rm {} \;
```
