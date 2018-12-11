# CS101A Assignment 11

> 11510225 Yuxing Hu (胡与兴)

**1. List the components of a typical operating system **

Shell, File manager, Device drivers, Memory manager, Scheduler, Dispatcher.

**2. What information is contained in a process table within an operating system?**

This entry contains such information as the memory area assigned to the process (obtained from the memory manager), the priority of the process, and whether the process is ready or waiting. 

**3. If each time slice in a multiprogramming system is 50 milliseconds and each context switch requires at most a microsecond, how many processes can the machine service in a single second?**

If each process consumed its entire time slice, the machine could provide a complete slice to almost 20 processes in one second. If processes did not consume their entire time slices, this value could be much higher, but then the time required to perform a context switch might become more significant.

**4. In a multiprogramming system, how can high-priority processes be allowed to run faster than others?** 

They could be given higher priorities so that they would be given prefer- ence by the dispatcher. Another option would be to give the higher-priority processes longer time slices. 

**5. Suppose three items R, S, and T are placed in a queue in that order. Then one item is removed from the queue before a fourth item, X, is placed in the queue. Then one item is removed from the queue, the items Y and Z are placed in the queue, and then the queue is emptied by removing one item at a time. List all the items in the order in which they were removed. **

RSTWYZ

**6. Suppose a multiprogramming operating system allocated time slices of 10 milliseconds and the machine executed an average of five instructions per nanosecond. How many instructions could be executed in a single time slice? **

1 millisecond = 1 * 10^-3 second

1 nanosecond = 1 * 10^-9 second

1 timeslice = 10 milliseconds = 10^7 nanosecond

10^7 * 5 = 5 * 10^7 instructions