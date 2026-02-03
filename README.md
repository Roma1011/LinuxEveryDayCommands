# LinuxEveryDayCommands

### Maintaining Processes and System Services

1) Sort By CPU usage
  - ps -e --format uid,pid,tty,%cpu,cmd --sort -%cpu
2) Sort By MEM Usage
  - ps -e --format uid,pid,tty,rss,cmd --sort -rss
3) Sum MEM Usage for a Specific User
  - ps -U user1 --format %mem | awk '{memory +=$1}; END {print memory}'
4) Sum MEM Usage for The Curent User
  - ps -U $USER --format %mem | awk '{memory +=$1}; END {print memory}'
5) Process Tree
  - pstree -p




### File viewing / File inspection
1) tail -f show loggs in live action
  - tail -f /var/log/nginx/access.log
