# bcc_tool-oomkill
An updated bcc oom_kill tool which successfully traces out of memory

Updated bcc oom_kill tool to successfully trace out of memory for kernel versions > 4.8

The bcc tool available till date supports from kernel version 4.4 to 4.8 and gives anamolous output as given below for OOM kill of PID and total_pages consumed 

17:39:52 Triggered by PID 10505 ("a.out"), OOM kill of PID 1835561760 ("lukB high:%lukB "), 2361183241434822607 pages, loadavg: 1.88 1.70 1.24 3/479 10508
