# Linux-Scheduler
The scheduleris modified so that when everytime a process is selected through the RB-tree,it is compared to all other process with soft-realtime requirements and seen which one of those  require the CPU more urgently than the one selected through the regular RB- tree. The one that urgently requires CPU time is scheduled before the  one selected through CFS.
