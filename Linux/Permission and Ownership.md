# 🔒 Linux File Permissions & Ownership

Understanding file permissions and ownership is essential for managing security in Linux. Every file and directory has specific permissions that define who can read, write, or execute it.

---

## 📜 1. Viewing File Permissions

To check file permissions, use:
```sh
ls -l filename
```
**Example Output:**
```sh
-rwxr-xr-- 1 user group 1234 Feb 15 12:00 myfile.sh
```
### Breakdown:
| Symbol | Meaning |
|--------|---------|
| `-` | Regular file (or `d` for directory) |
| `rwx` | Owner (read, write, execute) |
| `r-x` | Group (read, execute) |
| `r--` | Others (read only) |

---

## 🛠️ 2. Changing Permissions with `chmod`

### **Symbolic Mode:**
```sh
chmod u+x script.sh  # Add execute permission to user
chmod g-w file.txt   # Remove write permission from group
chmod o+r file.txt   # Give others read permission
```
### **Numeric (Octal) Mode:**
| Number | Permission |
|--------|------------|
| 7 | Read, Write, Execute (rwx) |
| 6 | Read, Write (rw-) |
| 5 | Read, Execute (r-x) |
| 4 | Read-only (r--) |
```sh
chmod 755 script.sh  # rwxr-xr-x (Owner: all, Group: read/execute, Others: read/execute)
chmod 644 file.txt   # rw-r--r-- (Owner: read/write, Group & Others: read)
```

---

## 👤 3. Changing Ownership with `chown`

### **Change File Owner:**
```sh
chown newuser file.txt
```
### **Change File Owner and Group:**
```sh
chown user:group file.txt
```
### **Recursively Change Ownership (for directories):**
```sh
chown -R user:group my_directory/
```

---

## 🎯 Summary
- Use `ls -l` to check permissions.
- `chmod` to modify file permissions (symbolic & numeric modes).
- `chown` to change file ownership.
