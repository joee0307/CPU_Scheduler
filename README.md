# CPU SCHEDULER

A brief description of what this project does and who it's for

# Overview

This repository contains a CPU Scheduler simulation implemented in Python. The simulation supports four scheduling algorithms:
1.) Shortest Job Next (SJN)
2.) Round Robin (RR). 
3.) Shortest Job First (SJF)
4.) Last Job First (LJF)

## Files
cpu_scheduler.cpp: The main C++ script containing the implementation of the CPU scheduling algorithms.

input.txt: The input file containing the list of jobs to be scheduled.

output.txt: The output file where the results of the scheduling are written.

# How to Run the Project
To run the project, follow these steps:

Clone the repository: git clone https://github.com/Deepak42-y/CPU-Scheduler.git
Compile the code: g++ -o cpu_scheduler cpu_scheduler.cpp
Run the executable: ./scheduler input.txt output.txt

# Internal Working
## SJF (Shortest Job First)
Arrival: Sort processes by arrival time.

Execution: Select the process with the shortest burst time among the arrived processes.

Completion: Calculate waiting time and turnaround time for each process.

Output: Output average waiting time and turnaround time.

## SRTF (Shortest Remaining Time First)
Arrival: Sort processes by arrival time.

Execution: Select the process with the shortest remaining time among the arrived processes.

Preemption: If a shorter job arrives, preempt the current job.

Completion: Calculate waiting time and turnaround time for each process.

Output: Output average waiting time and turnaround time.

## Round Robin
Arrival: Maintain a ready queue.

Execution: Execute each process for a fixed time quantum.

Preemption: If the process's quantum expires, move it to the end of the queue.

Completion: Calculate waiting time and turnaround time for each process.

Output: Output average waiting time and turnaround time.

## LJF (Longest Job First)
Arrival: Sort processes by arrival time.

Execution: Select the process with the longest burst time among the arrived processes.

Completion: Calculate waiting time and turnaround time for each process.

Output: Output average waiting time and turnaround time.

## Learning Takeaways

Understanding of different CPU scheduling algorithms and their implementation in C++.

Hands-on experience with process management and scheduling in an operating system.

Importance of algorithm choice in optimizing CPU utilization and response time.

## Resources/References

Operating System Concepts by Abraham Silberschatz, Peter Baer Galvin, and Greg Gagne

GeeksforGeeks articles on CPU Scheduling Algorithms
