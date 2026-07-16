# 06 - Process Management

## Objective

In this chapter, I learned how to monitor running processes, identify resource usage, and manage processes in Linux. I also learned the difference between foreground and background jobs.

---

## Commands Learned

### ps

Displays the running processes in the current terminal.

Example:

ps
---

### ps aux

Displays all running processes with detailed information.

Example:

ps aux
---

### top

Displays running processes in real time.

Useful for monitoring CPU and memory usage.

Example:

top
---

### kill

Terminates a process using its PID.

Example:

kill 3456
---

### kill -9

Forcefully terminates a process if it does not stop normally.

Example:

kill -9 3456
---

### jobs

Displays jobs running or stopped in the current terminal.

Example:

jobs
---

### bg

Resumes a stopped job in the background.

Example:

bg
---

### fg

Brings a background or stopped job back to the foreground.

Example:

fg
---

## Practice

- Used ps to view processes running in the current terminal.
- Used ps aux to display all running processes and identify CPU and memory usage.
- Used top to monitor processes in real time.
- Created a test process using:

sleep 300
- Found the process using:

ps aux | grep sleep
- Identified the process PID.
- Stopped the process using:

kill PID
- Practiced suspending a process using Ctrl + Z.
- Listed jobs using:

jobs
- Resumed a job in the background using:

bg
- Returned the job to the foreground using:

fg
---

## What I Learned

- The difference between ps and ps aux.
- How to identify a process using its PID.
- How to monitor system activity using top.
- The difference between stopping and killing a process.
- The difference between a Process and a Job.
- The difference between Foreground and Background execution.
- Why kill should be used before kill -9.

---

## Notes

- ps shows only processes running in the current terminal.
- ps aux shows all running processes on the system.
- top updates automatically and is useful for real-time monitoring.
- kill requests a process to terminate gracefully.
- kill -9 should only be used when a process does not respond.
- Ctrl + Z pauses a process; it does not terminate it.
- jobs works only with jobs in the current terminal session.
- bg resumes a stopped job in the background.
- fg brings a job back to the foreground.
