# Banker-s-Algorithm
Distributed Deadlock Detection Algorithm.

The banker’s algorithm is a resource allocation and deadlock avoidance algorithm that tests for safety by simulating the allocation for predetermined maximum possible amounts of all resources, then makes an “s-state” check to test for possible activities, before deciding whether allocation should be allowed to continue.
The algorithm employs several time varying data structures:

Available- A vector of length m indicates the number of available resources of each type.

Allocation- An n*m matrix defines the number of resources of each type currently allocated to a process. Column represents resource and resource represent process.

Request- An n*m matrix indicates the current request of each process. If request[i][j] equals k then process Pi is requesting k more instances of resource type Rj.

We treat rows in the matrices Allocation and Request as vectors, we refer them as Allocationi and Requesti.

Here we have 3 input matrix where max[][] - denotes maximum resources that will be required by processes allocate[][] - denotes currently allocated resources to processes avail[][] - denotes resources available in the system We will calculate need matrix and then try to allocate. I f we can allocate safely then give a suitable message.
