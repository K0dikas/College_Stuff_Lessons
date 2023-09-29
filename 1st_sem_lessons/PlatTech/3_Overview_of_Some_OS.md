###### Microsoft Windows Operating System
- *MS-DOS operating system*, which was a successful OS used on early *personal computers*.
- **Kernel Components of Microsoft Windows OS**:
	- `Windows Executive` - This contains the *core OS modules/services*:
		- *I/O manager* - This provides a framework through which *I/O* devices are accessible to applications.
		- *Cache Manager* - This improves the performance of file-based I/O by allowing recently referenced file data to `reside in the main memory for quick access`.
		- *Object Manager* - This creates, manages, and deletes Windows Executive objects that are used to represent resources such as processes, threads, and synchronization objects.
		- *Plug-and-play manager* - This determines which `drivers are required` to support a particular device and loads those drivers.
		- *Power Manager* - This coordinates the `power consumption` among various devices.
		- *Security reference monitor* - This `enforces the access` validation and audit-generation rules for all `protected objects` including files, processes, address spaces, and I/O devices.
		- *Virtual memory manager* - This manages `virtual addresses`, `physical memory`, and `paging files on a disk`.
		- *Process/thread manager* - This `creates`, `manages`, and `deletes` processes and thread objects.
		- *Configuration manager* - This is responsible for implementing and managing the `system registry`, which serves as the repository for both system-wide and per-user settings of various parameters.
		- *Advanced local procedure call (ALCP) facility* - This implements an efficient `cross-process call mechanism` for `communication` between local processes implementing services and subsystems.
	- `Windows Kernel` - This is considered the *core* software of the OS.
	- `Hardware abstraction layer (HAL)` - This *isolates* the OS f rom platform-specific hardware variances.
	- `Device Drivers` - These are *dynamic libraries* that extend the functionality of the Windows Executive.
	- `Windowing and Graphing System` - Implements *GUI*.
- **User mode processes**:
	- `Special system processes` - These include *user-mode services* such as the session manager, the authentication subsystem, the service manager, and the log-on process.
	- `Service processes` - These involve services used by both Microsoft and other external software developers to extend system functionality.
	- `Enviroment Subsystems` - These provide different *OS* environment and support *POSIX* and *Win32* subsystems.
	- `User applications` - These include *.EXE* programs and *DLLs* that provide the functionality a user needs to make use of a system.

###### Classic UNIX System
- Developed at *Bell Labs*.
- Written in `Assembly` and later converted to the `C Programming Language`.
- *Uniplexed Information and Computing Services (UNICS)*.
- Equipped with a number of user services:
	- `Shell` - This supports system calls from applications, other interface software, and the components of the `C Compiler`, such as the compiler itself, `Assembler`, and the `loader`.
- Designed to run on a *single processor*.
- **Three levels**:
	- `User Level` - Focuses on the linked programs and libraries.
	- `Hardware Level` - Focuses on the physical hardware and interface.
	- `System Kernel` - Focuses on the overall operation of the system.

###### Modern UNIX System
- There was a need to produce a new system implementation that would *unify* significant innovations and modern design features.
- The *Berkeley Software Distribution (BSD)* played an important role in the development of `UNIX OS` design theory.
- Common facilities exist which serve as a core of operating system, written a `modular fashion`.
	- `System V Release 4 (SVR4)` - By *AT&T* and *Sun Microsystems*.
	- The system kernel of this *OS* has a clean implementation.
	- Includes *real time processing support*, *process scheduling classes*.

###### Linux Operating System
- Started out as a `UNIX` variant for the `IBM PC architecture`, which was written by *Linus Torvalds*. Early version of Linux on the internet around `1991`.
- Free and open source variant of the UNIX OS.
- Composed of *independent blocks* called `loadable modules`, which can be *automatically loaded* and *unloaded* on demand.
	- `Dynamic Linking` - The modules can be `loaded` and `linked` into the kernel *while the kernel is already in memory and executing*.
	- `Stackable Modules` - The modules are arranged in hierarchical order. 
	- **Kernel Components of Linux OS**:
		- `System calls`
		- `Signals`
		- `Processes and scheduler`
		- `Virtual Memory`
		- `File Systems`
		- `Network Protocols`
		- `Physical Memory`

###### Android Operating System
- *Linux-based system* originally designed for mobile phones.
- *Does Not* contain drivers.
- *Android, Inc.,* which was bought by *Google* in `2005`.
- *Android Open-Source Project* `(AOSP)` source code.