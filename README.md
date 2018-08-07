# bcc_tool-oomkill
An updated bcc oom_kill tool which successfully traces out of memory for kernel versions > 4.8

The bcc tool available till date supports from kernel version 4.4 to 4.8 and gives anamolous output as given below for OOM kill of PID and total_pages consumed 

17:39:52 Triggered by PID 10505 ("a.out"), OOM kill of PID 1835561760 ("lukB high:%lukB "), 2361183241434822607 pages, loadavg: 1.88 1.70 1.24 3/479 10508.

But the kernel function oom_kill_process has been changed after 4.8 and hence modified bcc/oom_kill.py tool to trace out of memory for kernel versions till date!

Output after modifications for process a.out which consumed memory infinitely and got killed

23:38:03 Triggered by PID 22426 ("a.out"), OOM kill of PID 22426 ("a.out"), 4085393 pages, loadavg: 6.01 5.09 4.22 1/715 23199

