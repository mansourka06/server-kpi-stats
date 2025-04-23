# Server KPI Stats Monitor

![Bash](https://img.shields.io/badge/shell_script-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

`server-kips-stats.sh`  is a production-ready server KPI monitoring script that provides comprehensive system statistics with alerting capabilities. It provides a quick snapshot of your Linux server’s performance. It monitors CPU usage, memory stats, disk usage, and the top resource-consuming processes.

===============================

## OS Compatibility

- [x] Debian
- [x] Ubuntu  
- [x] RedHat/CentOS
- [x] Amazon Linux
- [ ] SUSE (untested)
- [ ] Arch Linux (untested)

## 📦 Dependencies

This script uses standard Linux tools:

- top
- awk
- sed
- grep
- bc
- ps
- df

No external packages required.

## Features

- 🖥️ Real-time CPU, memory, and disk usage monitoring
- 🚨 Threshold-based alerts and warnings
- 📊 Top processes by CPU and memory consumption
- 📈 Load average tracking
- 💾 Disk and inode usage monitoring
- 🎨 Color-coded output for quick status identification

## 📁 Script Overview

- 💻 CPU Usage - Uses top, grep, sed, and awk to extract CPU idle percentage and calculate actual usage.
- 🧠 Memory Usage - Parses /proc/meminfo to get: MemTotal, MemAvailable.
- 💾 Disk Usage - Uses df -h / and df / to get: Human-readable disk size and Used and available disk space in KB.
- 📌 Top Processes - Fetches the top 5 processes sorted by: CPU and Memory, through ps aux.

## Usage

### 1- Clone the script

```bash
curl -o https://github.com/mansourka06/server-kpi-stats.git
```

### 2- Make it executable

```bash
sudo chmod +x server-kpi-stats
```

### 3- Run the script

```bash
sudo ./server-kpi-stats.sh
```

## Pro tip

To monitor performance at intervals, set up a `cron job` like:

```bash
*/5* ** * /path/to/server-stats.sh >> /path/to/log.txt
```

## Author

[Mansour KA](https://github.com/mansourka06)