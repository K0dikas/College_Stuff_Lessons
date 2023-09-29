An *OS* controls all the events within a computer system.
- The following are the four different types of tables:
	1. **Memory Table** - These are used to keep track of both the `main` and the `secondary memory`.
	2. **I/O tables** - These are used by the OS to *manage input and output*  devices.
	3. **File Tables** - These tables hold information regarding the existence of files.
	4. **Process tables** - These tables are maintained by the *OS* to manage processes.
- `Process Location` - At a minimum, a process must include a program to be executed.
- `Process Images` - Process control blocks.
- `Process Attributes` - A *multi-programming system* requires a great deal of information about each process that resides in a process control block.
	- **Process Identification** - Unique numeric identifiers.
	- **Processor State Information** - Consists of processor registers' information.
	- **Process Control Information** - Contains additional information needed by the *OS* to control and coordinate.
- `User Mode` - This is referred to as the *less-priviledge mode*, since user programs execute in this mode.
- `Kernel Mode` - This is referred to as the *more-privileged mode*, where the software has complete control of the processor and its *instructions*, *registers*, and *memory*.
- `Process Creation` - When a new process is to be added to those currently being managed, the *OS* builds the data structure that will manage the *process and allocates address space in the main memory* for the process.
	1. *Assign a unique process identifier to the new process*
	2. *Allocate space for the process*
	3. *Initialize the process control block*
	4. *Set the appropriate linkages*
	5. *Create or expand other data structures*
- `Process Switching` - When the *OS* controls the currently running processes, a process switch may occur at any time.
	- `Interrupts` - are external events that are independent of the currently running process.
	- `Traps` - Are related *errors* conditions generated within the currently running process.
	- `Supervisor call` - Due to an explicit request can still occur to interrupt a process execution.
- `Process Termination` - Any computer system must provide means for a process to indicate its completion.