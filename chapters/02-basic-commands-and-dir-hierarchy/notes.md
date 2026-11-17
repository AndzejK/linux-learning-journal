## Navigating Directories

**Root Directory**: The Unix directory hierarchy starts at '**/**'.

## Variables (Shell VS Environment)
- **Shell var**: a *value* that belongs to my **current** shell
- **Env var**: a *value* that can be passed down to a program by my open shell session:

**Note**: Do Not put any space around the *=* when assingning a var!

```bash
EXPORT 
``` # exposes the var to global (env) scope

```bash
#!/bin/bash
export DEPLOY_ENV="PROD"
echo "Deploying to: $DEPLOY_ENV"
``` 
## Kernel Location
```bash
/boot/vmlinuz 
```
or
```bash
/vmlinuz /boot/vmlinuz 
```
- A *boot loader* loads this file into memory and sets it in motion when the system boots.
- Once the *boot loader* starts the kernel, the **main** kernel file is **no longer** used by the *running system*.

### Loadable Kernel Modules

```bash
/lib/modules 
```

```console
[rock@linux ~]$ ls -l /lib/modules/5.14.0-503.11.1.el9_5.x86_64/
total 27008
lrwxrwxrwx.  1 root root       45 Sep 30  2024 build -> /usr/src/kernels/5.14.0-503.11.1.el9_5.x86_64
-rw-r--r--.  1 root root   226297 Sep 30  2024 config
drwxr-xr-x. 13 root root      144 Jun 13 18:11 kernel
-rw-r--r--.  1 root root   887938 Jun 13 16:52 modules.alias
-rw-r--r--.  1 root root   840770 Jun 13 16:52 modules.alias.bin
-rw-r--r--.  1 root root      461 Sep 30  2024 modules.block
-rw-r--r--.  1 root root     9471 Sep 30  2024 modules.builtin
-rw-r--r--.  1 root root        0 Jun 13 16:52 modules.builtin.alias.bin
-rw-r--r--.  1 root root    11775 Jun 13 16:52 modules.builtin.bin
-rw-r--r--.  1 root root    77422 Sep 30  2024 modules.builtin.modinfo
-rw-r--r--.  1 root root   306695 Jun 13 16:52 modules.dep
-rw-r--r--.  1 root root   400940 Jun 13 16:52 modules.dep.bin
-rw-r--r--.  1 root root      387 Jun 13 16:52 modules.devname
-rw-r--r--.  1 root root      155 Sep 30  2024 modules.drm
-rw-r--r--.  1 root root       20 Sep 30  2024 modules.modesetting
-rw-r--r--.  1 root root     1664 Sep 30  2024 modules.networking
-rw-r--r--.  1 root root    93986 Sep 30  2024 modules.order
-rw-r--r--.  1 root root      918 Jun 13 16:52 modules.softdep
-rw-r--r--.  1 root root   511011 Jun 13 16:52 modules.symbols
-rw-r--r--.  1 root root   604240 Jun 13 16:52 modules.symbols.bin
lrwxrwxrwx.  1 root root        5 Sep 30  2024 source -> build
-rw-r--r--.  1 root root   308816 Sep 30  2024 symvers.gz
-rw-------.  1 root root  8876030 Sep 30  2024 System.map
drwxr-xr-x.  2 root root        6 Sep 30  2024 systemtap
drwxr-xr-x.  2 root root        6 Sep 30  2024 updates
drwxr-xr-x.  2 root root       40 Jun 13 18:11 vdso
-rwxr-xr-x.  1 root root 14456952 Sep 30  2024 vmlinuz
drwxr-xr-x.  2 root root        6 Jun 13 16:54 weak-updates
```

The `kernel` directory contains the **loadable kernel module** files. Files such as `modules.dep`, `modules.alias`, and `modules.symbols` contain module dependency and lookup information.