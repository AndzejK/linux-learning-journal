# `init` = **systemd**
- It is a user-space **program** like any other program on the Linux system, and you'll find it in `/sbin`:
```console
[rock@linux ~]$ ls -l /sbin/init 
lrwxrwxrwx. 1 root root 22 Apr  2  2026 /sbin/init -> ../lib/systemd/systemd
```
- It's basically a series of **scripts** that `init` runs, in sequence, one at a time.