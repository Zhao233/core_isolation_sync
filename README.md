# core_isolation_sync
This repository contains a tool that realize a core isolation(isolate specific processor core out of interrupt and scheduler subsystem) and strong synchronization between two specific process.    
This tool is implemented by add a system call to linux kernel, and works on aarch64.
## file discreption

### unistd.h
This file placed in $LINUX_KERNEL_PATH/include/uapi/asm-generic/.This file defined the mapping for system call number and ssystem call name 
### syscalls.h
This file placed in $LINUX_KERNEL_PATH/include/linux/.This file defined the system call function prototype 
### sys.c
This file palced in $LINUX_KERNEL_PATH/kernel/. This file contain the implementation of the system call function
