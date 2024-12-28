# sysopctl v0.1.0

`sysopctl` is a command-line tool designed to manage system resources, processes, and tasks on Linux systems. With this tool, you can perform operations such as listing services, monitoring disk usage, analyzing logs, and more.

---

## Installation Guide

### Step 1: Open WSL
Make sure you have a Linux environment set up using Windows Subsystem for Linux (WSL).

### Step 2: Clone the Repository
Clone the repository by running the following command:

```bash
git clone https://github.com/pandeyji2509/sysopctl
cd sysopctl
```

### Step 3: Move `sysopctl` to a System-Wide Path
To make `sysopctl` accessible as a system-wide command, move the script to a directory in your system's `PATH` (e.g., `/usr/local/bin`):

```bash
sudo mv sysopctl.sh /usr/local/bin/sysopctl
```

### Step 4: Make the Script Executable
Make the script executable with this command:

```bash
sudo chmod +x /usr/local/bin/sysopctl
```

### Step 5: Verify the Installation
Confirm the installation by checking the help documentation:

```bash
sysopctl --help
```

---

## Usage Guide

Once installed, you can use the `sysopctl` commands. Below are some of the operations you can perform:

### General Commands
1. Show help information:
   ```bash
   sysopctl --help
   ```

2. Display version details:
   ```bash
   sysopctl --version
   ```

### Service Management
1. List all active services:
   ```bash
   sysopctl service list
   ```

2. Start a service:
   ```bash
   sysopctl service start <service-name>
   ```

3. Stop a service:
   ```bash
   sysopctl service stop <service-name>
   ```

### System Monitoring
1. Check disk usage:
   ```bash
   sysopctl disk usage
   ```

2. Monitor real-time process activity:
   ```bash
   sysopctl process monitor
   ```

3. Analyze system logs:
   ```bash
   sysopctl logs analyze
   ```

### Backup System Files
Create backups of specified files or directories:
```bash
sysopctl backup <path>
```

---

## Example Commands

1. List running services:
   ```bash
   sysopctl service list
   ```

2. View disk usage:
   ```bash
   sysopctl disk usage
   ```

3. Start a service (e.g., `nginx`):
   ```bash
   sysopctl service start nginx
   ```

4. Backup a directory:
   ```bash
   sysopctl backup /home/user/documents
   ```

---
