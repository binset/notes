# data structure


hashtable

trees
* tree/balanced  AVL red/bloack tree
* tree traversal BFS DFS
* tree traversal inorder preorder postorder

graphs
* representation graphs with 
  * obj and pointer
  * matrix
  * adjacency list
* bfs traversal (complexity, tradeoffs)
* dfs traversal (complexity, tradeoffs)
* dijkstra
* a-star search

# algo
* complexity
* sorting merge quick

# cs
NP complete (Nondeterministic polynomial time)
* class P
  * class of questions for which some algorithm can provide an answer in polynomial time
* class NP 
  * class of questions for which an answer can be verified in polynomial time 
* class NP-Complete
  * Class of decision problems which contains the hardest problems in NP. 
  * Each NP-complete problem has to be in NP.
* class NP-Hard 
  * (non-deterministic polynomial acceptable problems)
  * Class of decision problems which are at least as hard as the hardest problems in NP. 
  * Problems that are NP-hard do not have to be elements of NP; 
  * indeed, they may not even be decidable.
* travelling salesman
* knapsack


# math
* itertools.permutations([1, 2, 3], 2)  # order matters
* itertools.combinations([1, 2, 3], 2)  # order doesn't matter



# OS
* processes, threads
  *  threads (of the same process) run in a shared memory space, while processes run in separate memory spaces.
* what resources a processes needs
  * A process has a virtual address space, executable code, open handles to system objects, a security context, 
  * a unique process identifier, environment variables, a priority class, minimum and maximum working set sizes, and at least one thread of execution. 
  * Each process is started with a single thread, often called the primary thread, but can create additional threads from any of its threads.
* what resources a thread needs
  * A thread is an entity within a process that can be scheduled for execution. 
  * All threads of a process share its virtual address space and system resources. 
  * In addition, each thread maintains exception handlers, a scheduling priority, thread local storage, a unique thread identifier, 
  * and a set of structures the system will use to save the thread context until it is scheduled. 
  * The thread context includes the thread's set of machine registers, the kernel stack, a thread environment block, 
  * and a user stack in the address space of the thread's process. 
  * Threads can also have their own security context, which can be used for impersonating clients.
* how context switching works
* how context switching is s initiated by the operating system and underlying hardware

# OS IPC
* locks (acquire, release) and mutexes 
* semaphores (like bike shed, only X number of bikes available)
  * internal counter which is decremented each time acquire() is called and incremented each time release() is called
* monitors (like toilet, only one person)
* deadlock and livelock (and how to avoid)
  * livelock = unable to make further progress. But threads are busy responding to each other and not blocked.
* Multithreading is concurrent and is used for IO-bound tasks
* Multiprocessing achieves true parallelism and is used for CPU-bound tasks
