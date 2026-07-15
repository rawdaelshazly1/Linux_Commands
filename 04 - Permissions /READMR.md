# 04 - Permissions

## Objective

In this chapter, I learned how Linux file permissions work and how to manage them using chmod and chown commands.

## Commands Learned

#### ls -l
- Displays file permissions, owner, group, and other file information.

Example:
ls -l
---

#### chmod
- Changes file or directory permissions.

Example:
chmod u+x script.sh

chmod g-w notes.txt

chmod a+r report.txt

chmod 755 script.sh

---

#### chown
- Changes the owner or group of a file.

Example:
chown root notes.txt

chown root:soc notes.txt

---

## Practice

- Viewed file permissions using ls -l.
- Identified the Owner, Group, and Others permissions.
- Changed file permissions using chmod.
- Changed the owner and group using chown.
- Practiced reading Linux permission strings.

---

## What I Learned

- Linux permissions are divided into Owner, Group, and Others.
- Read, Write, and Execute have different purposes.
- chmod changes permissions.
- chown changes the owner or group.
- Numeric permissions make it easier to assign multiple permissions at once.

---

## Notes

- Read = 4
- Write = 2
- Execute = 1

Common permission values:
- 7 = rwx
- 6 = rw-
- 5 = r-x
- 4 = r--
