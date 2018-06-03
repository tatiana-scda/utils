will set time clock on the motherboard into local time. Useful for time discrepancy in dual boot between Linux and Windows
```
timedatectl set-local-rtc 1 --adjust-system-clock
```

And to see the changes, look for RTC in local TZ: yes
```
timedatectl
```

To undo the operation, make RTF false
```
timedatectl set-local-rtc 0 --adjust-system-clock
 ```
