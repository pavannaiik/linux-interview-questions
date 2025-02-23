# Introduction to Linux

Linux is a Unix-like, open-source operating system widely used for servers, development, cloud computing, security, networking, and embedded systems.

## Why Learn Linux?
- ✔ Used in **Cloud Computing & DevOps**
- ✔ Powerful **CLI (Command Line Interface)**
- ✔ Runs on **Servers & Supercomputers**
- ✔ **Secure & Open-Source**
- ✔ **Customizable & Lightweight**

## Linux File System Structure
```
/      -> Root directory (everything starts here)
/home  -> User home directories
/etc   -> System configuration files
/bin   -> Essential binaries (commands like ls, cp, mv)
/usr   -> User programs and libraries
/var   -> Variable files like logs (/var/log)
/tmp   -> Temporary files
/dev   -> Device files (USB, HDD, etc.)
/proc  -> Process information (CPU, memory details)
```

## Basic Linux Commands

### 1. Navigation Commands
```
pwd        # Print the current working directory
ls         # List files and directories
cd ..      # Move one directory up
cd -       # Switch to the previous directory
cd ~/Documents -> Go to Documents folder
```

### 2. File and Directory Management
```
mkdir foldername  # Create a new directory
rmdir foldername  # Remove an empty directory
rm filename       # Delete a file
rm -r foldername  # Delete a directory and its contents
cp file1 file2    # Copy file1 to file2
mv oldname newname # Rename/move file
```

### 3. File Viewing & Editing
```
cat filename      # View file contents
less filename     # View large files page by page
head filename     # First 10 lines of file
tail filename     # Last 10 lines of file
nano filename     # Open file in Nano editor
vim filename      # Open file in Vim editor
```

### 4. User Management
```
whoami      # Show current user
who         # Show logged-in users
id          # Show user ID (UID) and group ID (GID)
adduser user # Add a new user
passwd      # Change user password
su user     # Switch user
sudo command # Run command as root
```

### 5. Process Management
```
ps aux      # Show running processes
top         # Monitor system processes
htop        # Interactive process viewer
kill PID    # Kill process with PID
pkill name  # Kill process by name
jobs        # Show background jobs
fg %1       # Bring background job to foreground
```

### 6. Disk Usage and Storage
```
df -h       # Show disk usage (human-readable)
du -sh dir  # Show directory size
```

### 7. Networking Commands
```
ifconfig / ip addr -> Show network interfaces
ping google.com    # Check connectivity
netstat -tulnp     # Show open ports
curl -O url        # Download file from the internet
```

### 8. Package Management

#### Debian/Ubuntu (APT)
```
sudo apt update  # Update package list
sudo apt install package_name  # Install a package
sudo apt remove package_name  # Remove a package
```

#### Red Hat/CentOS (YUM or DNF)
```
sudo yum install package_name
sudo dnf install package_name
```

#### Arch Linux (Pacman)
```
sudo pacman -S package_name
```

### 9. Permissions and Ownership
```
chmod 755 file   # Set file permissions
chown user:group file # Change file owner
ls -l            # View file permissions
```

### 10. Logs & System Monitoring
```
dmesg | less      # View system boot logs
journalctl -xe    # View system logs (for systemd)
uptime            # Show system uptime
free -h           # Show memory usage
```

## Conclusion
Linux is a powerful, stable, and secure OS with vast capabilities. Mastering Linux commands can boost productivity, enable automation, and help in system administration, DevOps, and cloud computing.
