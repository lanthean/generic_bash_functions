# generic_bash_functions

## Purpose
Set of bash functions useful at all times.

## Functions list
### log
Log messages with severity ([d]ebug|[i]nfo|[w]arning|[e]rror) to stdout or $LOG_FILE if set.  
```sh
log <severity> <message>
```
```
EXAMPLE
log i "This is a log message with severity info"

LOG_FILE will contain:
2019-04-02 14:02:53 CEST | ESC[0;32m[i]ESC[0m This is a log message with severity info

stdout will contain (while the [i] will be green):
2019-04-02 14:02:53 CEST | [i] This is a log message with severity info
```
### sys_log
Log message with severity prefix (debug|info|warning|error) to /var/log/local6.  
```sh
sys_log <severity> <message>
```
```
EXAMPLE
sys_log info "This is a log message with severity prefix info"

/var/log/local6 will contain:
2019-04-02T12:07:23.199934+00:00 rnd-vm-10-198 -bash[12662]: [info] This is a log message with severity prefix info
```

## Contact me
e	martin.bortel@gmail.com  
g https://github.com/lanthean  
