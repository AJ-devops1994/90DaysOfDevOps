Day 05 – Linux Troubleshooting Drill: CPU, Memory, and Logs

 systemctl status nginx
 ps -aux | grep nginx
 df -h
 du -sh /var/log/nginx
 clear
 ps -aux --sort=-%cpu | head -n 10
 df -h
 systemctl --failed
 ss -tunlp | tail