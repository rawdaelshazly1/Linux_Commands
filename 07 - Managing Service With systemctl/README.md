# 07 - Managing Service With systemctl

## Objective

In this chapter, I learned how to manage services in Linux using systemctl. I learned how to start, stop, restart, and reload services. I also learned how to enable services during boot and check their current status.

---

## Commands Learned

### systemctl status

Displays detailed information about a service.

Example:

systemctl status ssh
---

### systemctl start

Starts a stopped service.

Example:

sudo systemctl start ssh
---

### systemctl stop

Stops a running service.

Example:

sudo systemctl stop ssh
---

### systemctl restart

Restarts a service.

Example:

sudo systemctl restart ssh
---

### systemctl reload

Reloads the service configuration without stopping the service.

Example:

sudo systemctl reload ssh
---

### systemctl enable

Enables a service to start automatically during boot.

Example:

sudo systemctl enable ssh
---

### systemctl disable

Disables automatic startup during boot.

Example:

sudo systemctl disable ssh
---

### systemctl is-active

Checks whether a service is currently running.

Example:

systemctl is-active ssh
---

### systemctl is-enabled

Checks whether a service starts automatically during boot.

Example:

systemctl is-enabled ssh
---

### systemctl list-units --type=service

Displays active services.

Example:

systemctl list-units --type=service
---

### systemctl list-units --type=service --all

Displays both active and inactive services.

Example:

systemctl list-units --type=service --all
---

### systemctl list-unit-files --type=service

Displays installed service files and their startup state.

Example:

systemctl list-unit-files --type=service
---

## Practice

- Checked the status of the SSH service.
- Started and stopped the SSH service.
- Restarted the SSH service.
- Reloaded the SSH configuration.
- Enabled the SSH service to start during boot.
- Disabled automatic startup for the SSH service.
- Checked if the SSH service was active.
- Checked if the SSH service was enabled.
- Listed active services.
- Listed all services including inactive ones.
- Listed installed service files.

---

## What I Learned

- The difference between status and is-active.
- The difference between enable and start.
- The difference between disable and stop.
- The difference between restart and reload.
- How to check whether a service starts automatically during boot.
- How to display active services and all services.

---

## Notes

- status displays detailed information about a service.
- is-active quickly checks if a service is running.
- is-enabled checks whether a service starts automatically during boot.
- start starts a stopped service.
- stop stops a running service.
- restart stops and starts the service again.
- reload applies configuration changes without restarting the service.
- enable allows a service to start automatically during boot.
- disable prevents automatic startup during boot.
- list-units displays active services only.
- list-units --all displays both active and inactive services.
- list-unit-files displays installed service files and their startup state.
