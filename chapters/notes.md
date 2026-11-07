## Windows Environment:

- **IP:** 172.23.234.247

## MAC Environment:

- **IP:** 192.168.64.18

## Commands used to investigate the machine (RedHat Linux 9.8 (Plow))

- whoami
- id
- hostnamectl
- uname -a
- uptime
- free -h
- df -h
- systemctl --failed

## Commands used to investigate the Virtual Memory and CPU (RedHat Linux 10.2 (Coughlan))

### Start and Inspect two processes

```bash
sleep 600 &
P1=$!

sleep 600 &
P2=$!

echo "Process A: $P1"
echo "Process B: $P2"

ps -o pid,stat,comm -p "$P1,$P2"
```

1. `&` runs the command in the background.
2. `$!` captures the PID of the most recently started background process.
3. `P1` and `P2` hold the two process IDs.

### Inspect their virtual memory maps

```bash
head -n 12 /proc/$P1/maps
head -n 12 /proc/$P2/maps
```

### Compare the processes

```bash
grep -E '^(Name|Pid|VmSize|VmRSS):' /proc/$P1/status
grep -E '^(Name|Pid|VmSize|VmRSS):' /proc/$P2/status
```

- `VmSize`: total virtual memory size.
- `VmRSS`: resident memory currently occupying physical RAM.

### Checking Context Switching (cs)

```bash
vmstat 1 5
```
