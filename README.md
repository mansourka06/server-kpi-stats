# Server KPI Stats Monitor

![Bash](https://img.shields.io/badge/shell_script-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

A production-ready server KPI monitoring script that provides comprehensive system statistics with alerting capabilities.

## Features

- 🖥️ Real-time CPU, memory, and disk usage monitoring
- 🚨 Threshold-based alerts and warnings
- 📊 Top processes by CPU and memory consumption
- 📈 Load average tracking
- 💾 Disk and inode usage monitoring
- 🎨 Color-coded output for quick status identification

## OS Compatibility

- [x] Debian
- [x] Ubuntu  
- [x] RedHat/CentOS
- [x] Amazon Linux
- [ ] SUSE (untested)
- [ ] Arch Linux (untested)

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

## Author

[Mansour KA](https://github.com/mansourka06)