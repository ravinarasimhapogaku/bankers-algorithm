Q3. Write a multithreaded program that implements the banker's algorithm. Create n threads 
that request and release resources from the bank. The banker will grant the request only if it 
leaves the system in a safe state. It is important that shared data be safe from concurrent 
access. To ensure safe access to shared data, you can use mutex locks.
Ensure:
1. The program should be dynamic such that the threads are created at run time based on 
the input from the user. 
2. The resources must be displaced after each allocation. 
3. The system state should be visible after each allocation

Description:
The Banker's algorithm is a resource allocation and deadlock avoidance algorithm used in operating systems. It is designed to avoid deadlocks by ensuring that a safe state is always maintained.

The algorithm works by considering the current state of the system and the future requests for resources by each process. The system maintains information about the resources allocated to each process, the maximum resources required by each process, and the available resources in the system.

Based on this information, the algorithm determines if a request for resources can be granted without causing a deadlock. If the request can be granted, the resources are allocated to the process and the system state is updated. If the request cannot be granted, the process is blocked until the required resources become available.

To ensure a safe state, the algorithm uses a set of rules to determine if a request can be granted without causing a deadlock. A state is considered safe if there exists a sequence of process execution that allows all processes to complete their execution and release their resources without any deadlock.

Overall, the Banker's algorithm helps to prevent deadlocks by carefully managing resource allocation to ensure that the system is always in a safe state.
