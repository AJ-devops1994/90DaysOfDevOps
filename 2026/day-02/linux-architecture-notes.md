


========================================================================================
What systemd does and why it matters?
systemd: system and service manager
It provides a system and service manager that runs as PID 1 and starts the rest of the system.

systemd commands:
logs with journalctl:
journalctl -u <service> : view service logs
journalctl -b : logs since last boot
journalctl --since "10 minutes ago" : logs for a time range

System level commands: reboot/shutdown
systemctl reboot
systemctl poweroff

systemctl status: to check system status
systemctl status <service> : to check status of a particular service
systemctl start <service> 
systemctl stop <service>
systemctl restart <service>
systemctl enable <service> : to enable a service at boot
systemctl disable <service> : to disable a service at boot
systemctl reload <service> : Reload service config (no restart)
systemctl list-units --type=service : list running services
systemctl --failed : list failed services