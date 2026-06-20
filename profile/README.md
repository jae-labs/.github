<div align="center">

```
     ██╗ █████╗ ███████╗    ██╗      █████╗ ██████╗ ███████╗
     ██║██╔══██╗██╔════╝    ██║     ██╔══██╗██╔══██╗██╔════╝
     ██║███████║█████╗      ██║     ███████║██████╔╝███████╗
██   ██║██╔══██║██╔══╝      ██║     ██╔══██║██╔══██╗╚════██║
╚█████╔╝██║  ██║███████╗    ███████╗██║  ██║██████╔╝███████║
 ╚════╝ ╚═╝  ╚═╝╚══════╝    ╚══════╝╚═╝  ╚═╝╚═════╝ ╚══════╝
```

[![Website](https://img.shields.io/badge/justanother.engineer-f3eb2c?style=flat-square&logo=astro&logoColor=000)](https://justanother.engineer)
[![Uptime](https://img.shields.io/badge/uptime_stats-00ffff?style=flat-square&logo=statuspage&logoColor=000)](https://stats.pingdom.com/ieq3v42yov76/4989186)
[![Sponsor](https://img.shields.io/badge/buy_me_a_coffee-FFDD00?style=flat-square&logo=buymeacoffee&logoColor=000)](https://buymeacoffee.com/luiz1361)

</div>

---

### `/home/lui.z/$` `cat` `/etc/motd`

```
*******************************************************************************
*                                   WARNING                                   *
*                                                                             *
*  You are entering the jae-labs R&D organization                             *
*                                                                             *
*  Access is fully permitted. Unauthorized copying, modification, and         *
*  forking of any configuration or code are highly encouraged.                *
*                                                                             *
*  All connections are welcomed. Activity is monitored only to ensure         *
*  our automated pipelines don't collapse under their own weight.             *
*                                                                             *
*  Disconnect immediately if you are allergic to YAML indentation.            *
*  Otherwise, enjoy your stay!                                                *
*                                                                             *
*******************************************************************************
```

---

### `/home/lui.z/$` `who`

```bash
lui.z         web      Jun  4 07:56
```

---

### `/home/lui.z/$` `uname`

```bash
Darwin
```

---

### `/home/lui.z/$` `uptime`

```bash
20:17  up 37 years, 1 user, load averages: 2.55 2.13 2.13
```

---

### `/home/lui.z/$` `tree`

```bash
.
├── .github             # Organization-wide shared templates & profile
├── ansible             # Systems configuration management & playbooks
├── concierge           # Slack ChatOps bot in Go for provisioning automation
├── dotfiles            # Workstation bootstrapping config files for macOS
├── flashcards          # Privacy-first offline local AI study assistant
├── grafana-git-sync    # Bi-directional Grafana dashboard sync utility
├── homebrew-formulae   # Homebrew tap for custom packages
├── pages               # Source code for the justanother.engineer website
├── sandbox             # Experimental playground for unverified configurations
├── scripts             # Collection of handy helper utility scripts
├── skills              # Reusable agent skills and custom capabilities
├── template            # Generic Project Horizon repository template
└── terraform           # Core IaC modules and configurations

13 directories, 0 files
```
---

### `/home/lui.z/$` `crontab` `-l`

```bash
# 8:00 AM: send wake-on-lan (WOL) packet to host
0 8 * * *     wakeonlan ca:fe:ca:fe:ca:fe

# 8:55 AM: create tmux focus session if missing
55 8 * * 1-5  tmux has-session -t BUI 2>/dev/null || tmux new-session -d -s BUI

# 9:00 AM: run focus loop from system root
0 9 * * 1-5   tmux send-keys -t BUI 'cd / && while true; do make nice-things; sleep 300; done' C-m

# 1:00 PM: suspend focus loop & make lunch
0 13 * * 1-5  tmux send-keys -t BUI C-z && tmux send-keys -t BUI 'cd / && make lunch' C-m

# 2:00 PM: resume focus loop after lunch
0 14 * * 1-5  tmux send-keys -t BUI 'fg' C-m

# 5:00 PM: suspend loop & stop active make jobs
0 17 * * 1-5  tmux send-keys -t BUI C-z && pkill -f 'make nice-things'

# 11:00 PM: hibernate system
0 23 * * *    pmset sleepnow
```
