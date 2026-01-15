🚀 Day 5: System Monitoring & Service Management
📅 Date: January 15, 2026
🎯 Plan vs Reality

What I planned to do:

Complete 5 practical Linux exercises

Understand systemd services

Learn system monitoring with top

What actually happened:
✅ Completed all 5 exercises successfully
✅ Discovered SSH isn't installed in my WSL (surprise!)
✅ Monitored system health and understood load average

💡 Key Learnings
1. Services ≠ Processes
systemctl list-unit-files shows Docker services (enabled), while ps aux shows Docker processes. Different perspectives, same system.

2. Load average demystified
0.01, 0.01, 0.00 means my system is nearly idle. This simple metric tells the whole story of system health.

3. Default configurations vary
Not having SSH installed in WSL Ubuntu taught me: always check what's actually there, not what "should" be there.

🛠 Technical Progress
Service management:

bash
# Found Docker services
systemctl list-unit-files | grep docker
# docker.service - enabled
# docker.socket - enabled

# Checked service status
systemctl status systemd-logind
# Active: running (managing user logins)
System monitoring:

bash
# Real-time monitoring
top
# Load average: 0.01, 0.01, 0.00
# Total processes: 44
# Highest CPU: PID 2788

# Quick checks
uptime
free -h
🔄 The DevOps Mindset
Today's realization:
Setting wrong permissions (Exercise 2) was my most valuable lesson. In DevOps, catching your own mistakes before they reach production is the real skill.

Next: Networks, Docker, and building my first project — the journey continues!


