# 05 - Users & Groups

## Objective

In this chapter, I learned how Linux users and groups work, how to identify the current user, and why root and sudo are important for system administration and security.

## Commands Learned

#### whoami
- Displays the current logged-in user.

Example:
whoami
---

#### groups
- Displays all groups that the current user belongs to.

Example:
groups
---

#### id
- Displays user identity information such as UID, GID, and groups.

Example:
id
---

#### cat /etc/passwd
- Displays information about users stored on the system.

Example:
cat /etc/passwd
---

#### sudo
- Runs a command with elevated (root) privileges.

Example:
sudo apt update
sudo apt install wireshark
---

## Practice

- Identified the current user.
- Displayed user groups.
- Viewed user identity information.
- Explored the list of system users.
- Understood when and why to use sudo.

---

## What I Learned

- Every user should have a separate account.
- The root user has the highest privileges.
- whoami shows the current user.
- groups shows the user's groups.
- id provides detailed identity information.
- sudo allows authorized users to execute commands with root privileges.

---

## Notes

- Avoid working as root unless necessary.
- Follow the Principle of Least Privilege.
- Use sudo only when administrative privileges are required.
