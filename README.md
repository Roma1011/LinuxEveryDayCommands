# LinuxEveryDayCommands

### Maintaining Processes and System Services

1) Sort By CPU usage
  - ps -e --format uid,pid,tty,%cpu,cmd --sort -%cpu
2) Sort By MEM Usage
  - ps -e --format uid,pid,tty,rss,cmd --sort -rss
