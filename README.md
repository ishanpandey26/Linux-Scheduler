# Linux-Scheduler
Added a soft real-time requirement to a process – each process, that requires soft real-time guarantees must receive atleast x units of time-slice. Every time the scheduler is called, it is checked if the real-time guarantees of process with soft-realtime requirements are being met or not. Higher priority is given to a
process's soft-realtime requirement compared to the vruntime that is normally considered.
The scheduler is modified so that when everytime a process is selected through the RB-tree,it is compared to all other process with soft-realtime requirements and seen which one of those  require the CPU more urgently than the one selected through the regular RB- tree. The one that urgently requires CPU time is scheduled before the  one selected through CFS.
