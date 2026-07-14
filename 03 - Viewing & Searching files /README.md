# 03 - Viewing & Searching Files

## Objective

In this chapter, I learned how to view file contents and search inside files using Linux commands.

## Commands Learned

#### cat
- Displays the entire content of a small file.
- Best used with small files.

Example:
cat auth.log
#### less
- Opens large files page by page.
- Useful for reading and searching inside files.

Example:
less auth.log
Useful keys:
- Space → Next page
- b → Previous page
- / → Search
- q → Quit

#### head
- Displays the first 10 lines by default.

Example:
head auth.log
head -n 20 auth.log
#### tail
- Displays the last 10 lines by default.

Example:
tail auth.log
tail -n 15 auth.log
tail -f auth.log
#### grep
- Searches for specific text inside a file.

Example:
grep "Failed" auth.log
grep -c "Failed" auth.log
grep -i "failed" auth.log
#### find
- Searches for files by name.

Example:
find . -name "auth.log"
find /var/log -name "*.log"
## Practice

I created a simple log file and practiced viewing and searching its content.

## What I Learned

- cat is better for small files.
- less is better for large files.
- grep helps me search inside log files.
- tail -f is useful for monitoring logs.
- find helps me locate files quickly.

## Notes

- grep is case-sensitive by default.
- Use -i to ignore uppercase and lowercase letters.
- head and tail display 10 lines by default.
