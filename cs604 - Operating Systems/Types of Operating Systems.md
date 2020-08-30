## Higher Level Components of computer system
1. **Hardware**
2. **Operating System**
    manages use of hardware among the various application programs for users.
3. **Application Programs**
    softwares used by users (compilers, database systems, video games, business programs)
4. **Users** are people, machines, and other computers

## Types of Operating System

1. Single-User systems
2. Batch systems
3. Multi programmed systems
4. Time-sharing systems
5. Real Time systems

### Single-user Systems
- one user at a time
- **Goal**: maximize convenience and responsiveness instead of max utilization of cpu and devices
- They can urn **DOS**, **Windows**, **MacOS** and **Unix/Linux**

### Batch Systems   
- They were large old systems where input was card readers, tape etc and output was punch card,line printers, tape etc.
- User could not directly use it via console. Not interactive
- You had to prepare a job (consists data,program and control information) in form of punch cards and submit to computer operator
- For speed: operator batch together jobs with similar needs.
- Fortran programs were compiled one after another
- In such systems cpu is often idle because the speed of mechanical I/O.
- **systems in which the user does not get to interact with his/her jobs and jobs with similar needs are executed in a “batch”, one after
the other, are known as batch systems**
- Example Digital Equipment Corporation's VMS OS
  
### Multi-programmed systems
- **Increase CPU utilization** by organizing jobs so that CPU always has one to execute
- Keep several jobs in memory
- Jobs in memory are subset of jobs on harddisk which are ready but can't be loaded to memory yet
- when a job needs to wait (because of I/O), cpu simply switches to another job
- All jobs that enter the system are kept in **job pool**
- Job pool consists of all jobs on dist awaiting to be loaded in memory.
- If several jobs are ready to be loaded into memory, and there is not enough room for all of them, then the system
must choose among them. This decision is called **job scheduling**
- if several jobs are ready to run at the same time, the system must choose among them. 
CPU must choose among them, it is called **CPU scheduling**

### Time-sharing Systems
- Multi-user, Multi-process, Interactive
- Uses **Multi-programming** and **CPU scheduling**
- CPU scheduling to provide each user portion of time-shared computer
- **Unix/Linux**, **Windows NT Server**, and **Windows 2000 server**

### Real Time systems
- used in rigid time requirements
- often used as control device in a dedicated applications
- Example: Systems that control scientific experiments, medical imaging, industrial control systems
- Has well defined, fixed time constraints
- **If system does not produce output for an input within a time constraint, system will fail.**
- Types:
  - **Hard**: guarantees that critical tasks be completed on time.
    - This goal requires that all delays in system be completed on time.
    - OS kernel delays need to be bounded
    - Secondary storage is either limited or missing
    - data stored in short-term memory on in ROM
    - Most advanced OS features are missing too
    - Hard real-time sytem can't be mixed with other types of systems


  - **Soft**: less restrictive
    - critical real-time tasks gets priority and retains until completion 
    - OS kernel delays need to be bounded
    - Soft real-time system can be mixed with other types of systems