- The term `process` can be defined in different ways, depending on its actual composition or utilization.
	- A `process` can be a program in execution.
	- A `process` can be an instance of a program running on a computer.
	- A `process` can be considered as an entity that can be assigned to and executed on a processor.
	- A `process` can be treated as a unit of activity that executes a sequence of instructions, a current state, and an associated set of system resources.
	- A `process` can also be defined as an environment that consists of a number of elements for executing a user-level program.
- *Two Essential elements*:
	- `Program Code`: Can be shared with other processes that are executing the same program, and the *set of data* associated with the program code.
- The process itself cat be uniquely characterized by the following elements:
	- `Identifier` - It is a unique identifier for each process.
	- `Process State` - It indicates the current activity of a process.
		- *New* - The process is being created.
		- *Ready* - The process is waiting to be assigned to a processor.
		- *Running* - The instructions are being executed.
		- *Waiting* - The process is waiting for a particular event to occur.
		- *Terminated* - The process has finished the execution.
	- `Priority` - Priority level relative to other processes.
	- `Program counter` - Indicates the *address* of the next instruction to be executed for a particular process.
	- `Memory Pointer` - Contains pointers to program codes and data associated with the process, including any memory blocks shared with other processes.
	- `Context Data` - These are the data present in a processor's registers during process execution.
	- `I/O status information` - This includes different information associated with the *input/output* status of a process.
	- `Accounting information` - This includes different tracking information
	- associated with the process, such as the amount of *processor time*, the *clock time* used, and *time limits*.
- **Process control block** - The elements of a process are stored in a data structure.

###### Two-state Process model
- An *OS* controls the course of execution that involves the process of determining an interleaving pattern for execution and allocating resources to processes.
	- `Not Running State` - When the *OS* creates a new process, it creates a process control block for the new process and adds the new process into the not running state of the system.
	- `Running State` - The dispatch portion of the *OS* selects a particular process to run. Then, in enters the running state.

###### Five-State Process Model
- This model *naturally* handles processes through the implementation of `five unique states`:
	- `New State` - A process that has just been created and has not yet been admitted to the pool of executable processes by the *OS*.
	- `Ready State` - A process that is prepared to execute when given the opportunity.
	- `Running State` - A process that is currently being executed.
	- `Blocked State/Waiting State` - A process that cannot execute until some event occurs, such as the completion of an *I/O operation*.
	- `Exit State` - A process that has been released from the pool of executable processes by the *OS*, either because it halted or it was terminated.

###### Suspended Processes
- `Ready, Running, and Blocked`, provide a systematic way of modelling the behavior of a process and guide the implementation of an operating system.
- In a `suspended process model`, processes that are not immediately available for execution can occur.
	- *The process itself*
	- *A parent process*
	- *The Operating System*