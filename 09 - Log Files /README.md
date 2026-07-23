# 09 - Log Files

## Objective

In this chapter, I learned how Linux stores system logs, how to monitor log files, and how to investigate system events using different log files and log management commands.

---

## Commands Learned

### /var/log

The main directory that contains most system log files.

Example:

cd /var/log
---

### auth.log

Stores authentication-related logs, including successful and failed logins, SSH activity, and sudo usage.

Example:

less /var/log/auth.log
---

### syslog

Stores general system and service logs.

Example:

less /var/log/syslog
---

### tail

Displays the last 10 lines of a file by default.

Example:

tail /var/log/syslog
---

### tail -f

Monitors a log file in real time and displays new log entries as they are written.

Example:

tail -f /var/log/auth.log
---

### journalctl

Displays logs collected by systemd.

Example:

journalctl
---

### journalctl -xe

Displays the most recent log entries with additional explanations for troubleshooting.

Example:

journalctl -xe
---

### journalctl -u

Displays logs for a specific service.

Example:

journalctl -u ssh
---

### dmesg

Displays kernel messages related to hardware and system startup.

Example:

dmesg
---

### last

Displays the login history of users.

Example:

last
---

## Practice

- Navigated to the log directory using:

cd /var/log
- Explored authentication logs using:

less /var/log/auth.log
- Explored general system logs using:

less /var/log/syslog
- Displayed the last log entries using:

tail /var/log/syslog
- Monitored log files in real time using:

tail -f /var/log/auth.log
- Viewed systemd logs using:

journalctl
- Displayed the latest log entries for troubleshooting using:

journalctl -xe
- Viewed logs for a specific service using:

journalctl -u ssh
- Displayed kernel messages using:

dmesg
- Viewed user login history using:

last
---

## What I Learned

- Most Linux log files are stored in /var/log.
- auth.log stores authentication-related events.
- syslog stores general system and service events.
- The difference between tail and tail -f.
- How journalctl simplifies viewing system logs.
- When to use journalctl -xe for troubleshooting.
- How to display logs for a specific service using journalctl -u.
- dmesg displays kernel and hardware-related messages.
- last displays user login history.

---

## Notes

- /var/log contains most system log files.
- auth.log records successful and failed logins, SSH activity, and sudo usage.
- syslog records general system events and service logs.
- tail displays the last lines of a log file once.
- tail -f monitors a log file continuously in real time.
- journalctl displays logs collected by systemd.
- journalctl -xe is useful for investigating recent system issues.
- journalctl -u service_name displays logs for a specific service.
- dmesg is commonly used to troubleshoot hardware-related issues.
- last displays the history of successful user logins.
