# Important Operating System Algorithms

## 1. Process Scheduling Algorithms
- **First-Come, First-Serve (FCFS)**: The simplest scheduling algorithm where processes are scheduled in the order they arrive.
- **Shortest Job First (SJF)**: Prioritizes processes with the shortest burst time; can be preemptive or non-preemptive.
- **Round Robin (RR)**: Allocates a fixed time slice (quantum) to each process in a cyclic order.
- **Priority Scheduling**: Schedules processes based on priority, where higher-priority processes are executed first.
- **Multilevel Queue Scheduling**: Separates processes into multiple queues based on specific criteria (e.g., foreground vs. background processes).

## 2. Memory Management Algorithms
- **Paging**: Implement simple paging to simulate how memory is divided into fixed-size pages and mapped to frames.
- **Segmentation**: Demonstrates the allocation of memory based on segments, representing different parts of a process.
- **Page Replacement Algorithms**:
  - **First-In, First-Out (FIFO)**: Replaces the oldest page in memory.
  - **Least Recently Used (LRU)**: Replaces the page that hasn’t been used for the longest time.
  - **Optimal Page Replacement**: Replaces the page that will not be used for the longest time in the future (often theoretical but good to know).
  - **Least Frequently Used (LFU)**: Replaces pages based on usage frequency.

## 3. Disk Scheduling Algorithms
- **First-Come, First-Serve (FCFS)**: Serves disk requests in the order they arrive.
- **Shortest Seek Time First (SSTF)**: Selects the request closest to the current head position.
- **SCAN (Elevator Algorithm)**: Moves the head towards one end, serving requests in that direction, then reverses.
- **C-SCAN (Circular SCAN)**: Similar to SCAN but only serves requests in one direction, then resets to the beginning.
- **LOOK and C-LOOK**: Variants of SCAN and C-SCAN that only go as far as the last request in each direction.

## 4. Deadlock Detection and Avoidance Algorithms
- **Banker’s Algorithm**: Checks if allocating resources to a process will keep the system in a safe state, helping in deadlock avoidance.
- **Deadlock Detection Algorithm**: Monitors system states and periodically checks for cycles among processes to detect deadlock.
- **Resource Allocation Graph (RAG)**: Used to represent and analyze potential deadlocks in resource allocation.

## 5. Synchronization Algorithms
- **Semaphore Implementation**: Use semaphores for process synchronization to avoid race conditions.
- **Mutex Locks**: Implement mutual exclusion to handle critical sections in concurrent programming.
- **Dining Philosophers Problem**: A classic synchronization problem that helps in understanding deadlock, starvation, and concurrency.
- **Producer-Consumer Problem (Bounded Buffer Problem)**: Demonstrates synchronization in a shared buffer between producers and consumers.
- **Readers-Writers Problem**: Illustrates synchronization between readers and writers to prevent data inconsistency.

## 6. File System Algorithms
- **File Allocation Methods**:
  - **Contiguous Allocation**: Files are stored in contiguous blocks on disk.
  - **Linked Allocation**: Files are stored in scattered blocks with each block pointing to the next.
  - **Indexed Allocation**: Uses an index block to maintain pointers to each block of a file.
- **Free Space Management**:
  - **Bit Vector**: Tracks free space on a disk with bits.
  - **Linked List Free Space Management**: Tracks free blocks using linked lists.

## 7. CPU Scheduling Algorithms
- **Multi-Level Feedback Queue (MLFQ)**: A complex CPU scheduling algorithm that uses multiple queues with different priorities.
- **Completely Fair Scheduler (CFS)**: Used in Linux, this scheduler divides CPU time equally among processes based on their weights.
