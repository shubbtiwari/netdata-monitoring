# Netdata Monitoring Task

##  Overview
This project demonstrates setting up **Netdata** for real-time system monitoring using **Docker**.  
Netdata provides second-by-second insights into system performance, including CPU usage, memory usage, disk I/O, network activity, and container statistics.

---

##  Tools Used
- **Docker** (for containerized Netdata deployment)
- **Netdata** (real-time monitoring tool)
- **Web Browser** (to view the dashboard)

---

##  Steps Followed

###  Run Netdata in Docker
```bash
docker run -d --name=netdata -p 19999:19999 --cap-add=SYS_PTRACE --security-opt apparmor=unconfined netdata/netdata
## Access the Dashboard
http://localhost:19999
Explore Metrics

CPU usage

Memory usage

Disk read/write activity

Network traffic

Docker container statistics
