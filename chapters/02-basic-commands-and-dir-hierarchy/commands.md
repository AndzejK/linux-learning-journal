## Intermediate Commands

### **grep**
Reads the **content** from a file or input stream and can match a filename too.

```bash
grep root /etc/passwd
```
### **diff**
Check the differences between two text files.

```bash
diff -u file.2 file.1
```

### Having the same shell session but launching/having a different session (**a child session**):
```bash
bash -c 'echo different session ID'
```