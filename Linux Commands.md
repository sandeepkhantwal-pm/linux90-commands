# Heading 1 (Creating 90% workable skills for various sets )

Various commands for the linux :--
Or Top 
Cheat Sheet for the top Linux commands to do :--


Essential command for the linux cover the 90%




## Directory and Navigation related commands :--
pwd          # Print current working directory
ls           # List files and directories
cd           # Change directory
mkdir        # Create directory
rmdir        # Remove empty directory
tree         # Display directory tree (if installed)

## File Management commands :--
touch        # Create empty file or update timestamp
cp           # Copy files/directories
mv           # Move/rename files/directories
rm           # Remove files/directories
ln           # Create links (hard/soft)
chmod        # Change file permissions
chown        # Change file owner
find         # Search for files
locate       # Find files by name (faster than find)
du           # Disk usage
df           # Disk free space

# Text Processing commands :--
cat          # Concatenate and display files
more/less    # View file contents page by page
head         # Display first lines of file
tail         # Display last lines of file
grep         # Search text using patterns
sed          # Stream editor for text manipulation
awk          # Text processing and reporting
sort         # Sort lines of text
uniq         # Remove duplicate lines
wc           # Word, line, character count
cut          # Remove sections from lines
paste        # Merge lines of files

# System Information commands :--
uname        # Print system information
whoami       # Display current user
id           # Display user identity
date         # Display/set date and time
cal          # Display calendar
uptime       # System uptime
free         # Memory usage
top/htop     # Process monitor
ps           # Process status
kill         # Kill processes
pkill        # Kill processes by name
bg/fg        # Background/foreground jobs
jobs         # List jobs

# Networking commands :--
ifconfig/ip  # Network interface configuration
ping         # Test network connectivity
traceroute   # Trace packet route
netstat/ss   # Network statistics
curl/wget    # Download files from web
ssh          # Secure shell connection
scp          # Secure copy over SSH
rsync        # Remote file sync
nmap         # Network exploration tool
dig          # DNS lookup
host         # DNS lookup utility

# Package Management (varies by distro) :--
apt (Debian/Ubuntu): install, update, upgrade, remove, search
yum/dnf (RedHat/CentOS/Fedora): install, update, upgrade, remove
pacman (Arch): -S (install), -Syu (update), -R (remove)
snap/flatpak # Universal package managers

# Compression and Archiving :--
tar          # Archive files
gzip/gunzip  # Compress/decompress files
zip/unzip    # Zip compression
bzip2/bunzip2 # Bzip2 compression

# User Management :--
useradd      # Add user
usermod      # Modify user
userdel      # Delete user
passwd       # Change password
su           # Switch user
sudo         # Execute as superuser
groups       # Show user groups

# System Administration :--
systemctl    # Control system services
journalctl   # Query systemd journal
crontab      # Schedule tasks
mount/umount # Mount/unmount filesystems
fdisk        # Disk partitioning
mkfs         # Create filesystem
shutdown     # Shutdown system
reboot       # Reboot system

# Miscellaneous :--
echo         # Display text
history      # Command history
alias        # Create command aliases
export       # Set environment variables
source/.     # Execute shell script
man          # Manual pages
info         # Info documentation
which        # Locate command
type         # Command type
time         # Time command execution
watch        # Execute command periodically

# These commands cover approximately 90% of common Linux tasks. Practice them in a safe environment!



Advance Commands :-----

File Editing commands :--
nano         # Simple text editor (easy for beginners)
vim/vi       # Powerful modal text editor
emacs        # Extensible text editor
gedit        # GUI text editor (GNOME)
kate         # GUI text editor (KDE)
code         # VS Code (if installed)
sed -i       # Edit files in-place with sed

File Transfer and Remote Operations :--
scp          # Secure copy files over SSH (scp file.txt user@host:/path)
rsync        # Advanced file sync with compression/delta (rsync -avz file.txt user@host:/path)
sftp         # Secure FTP client (interactive file transfer)
ftp          # Traditional FTP client
wget         # Download files from web/ftp
curl         # Transfer data with various protocols
ssh          # Secure shell connection (ssh user@host)
ssh-keygen   # Generate SSH keys for passwordless login
ssh-copy-id  # Copy SSH public key to remote host

Common Use Cases for Linux Server Environment :--
# Remote server management
ssh user@server.com
sudo apt update && sudo apt upgrade  # Update server packages

# File backup and sync
rsync -avz /local/dir user@backup:/remote/dir
tar -czf backup.tar.gz /important/files  # Create compressed backup

# Log monitoring
tail -f /var/log/syslog  # Follow system logs
journalctl -u service-name  # View systemd service logs

# Process monitoring and management
top  # Real-time process viewer
ps aux | grep process-name  # Find specific processes
kill -9 PID  # Force kill process
systemctl restart service  # Restart services

# Network troubleshooting
ping google.com  # Test connectivity
netstat -tlnp  # List listening ports
ss -tlnp  # Modern netstat alternative
curl -I http://localhost  # Check web server response

# Disk and filesystem management
df -h  # Check disk usage
du -sh /directory  # Directory size
fdisk -l  # List disk partitions
mount /dev/sdb1 /mnt  # Mount external drive

# Security and permissions
chmod 644 file.txt  # Set file permissions
chown user:group file.txt  # Change ownership
ufw status  # Check firewall status (Ubuntu)
firewall-cmd --list-all  # Check firewall (CentOS/RHEL)

# Cron jobs for automation
crontab -e  # Edit cron jobs
# Example: 0 2 * * * /path/to/backup-script.sh  # Daily backup at 2 AM

# Package installation and updates
# Debian/Ubuntu: apt install package-name
# CentOS/RHEL: yum install package-name or dnf install package-name
# Arch: pacman -S package-name

