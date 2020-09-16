# Linux Directory Structure

## **`/`**

 root directory is similar to a drive letter in Windows (C:\, D:\, etc.) except that in the Linux directory structure there is only one root directory. Typically no files or programs are stored directly under root

## **`/bin`**

  holds binary executable files that are essential for correct  
operation of the system. These binaries are usually available for  
use by all users. **`/usr/bin`** can also be used for this purpose as well

## **`/boot`**

 holds **essential system boot files** including the **kernel**  
image .

## **`/dev`**

 holds **devices**.  **Remember that Linux treats devices like files** and you can read and write to them as if they were. Included in this directory is the notorious /dev/null, which is most useful for deleting outputs of various, functions and programs.

## **`/etc`**

 holds **system configuration files**. 
 **Most files in this directory are text** and can be edited with your favorite text editor. 

- **`/etc/inittab`** is a text file that details what processes are started at system boot up and during regular operation. 
- **`/etc/fstab`** identifies file systems and their mount points (like floppy, CD-ROM, and hard disk drives). 
- **`/etc/passwd`** is where users are defined

## **`/home`**

 This is where every user on a Linux system will have a **personal directory**. A quick way to return to your home directory is by entering the "cd" command. Your current working directory will be changed to your home directory.

## **`/lib`**

**Shared libraries** and **kernel modules** are stored in this directory.The libraries can be dynamically linked which makes them very similar to DLL files in the Windows environmen


## **`/lost+found`**

 This is the directory where Linux keeps files that are restored after a crash  
or when a partition hasn't been unmounted properly before a shutdown.

## **`/mnt`**

Used for **mounting temporary filesystems**. Filesystems can be mounted  
anywhere but the /mnt directory provides a convenient place in the Linux  
directory structure to mount temporary file systems

## **`/opt`**

Often used for **storage of large applications** packages

## **`/proc`**

This is a special, **"virtual"** directory where **system processes are stored**.  
This directory doesn't physically exist but you can often view (or read) the  
entries in this directory.

## **`/root`**

The home directory for the superuser (root).  `/` and `/root` are not same.

## **`/sbin`**

**System administration utilities**  (halt, ifconfig, fdisk, etc.) are
stored in this directory. `/usr/sbin`, and `/usr/local/sbin` are other directories that are used for this purpose as well. `/sbin/init.d` are scripts used by 
`/sbin/init` to start the system.

## **`/tmp`**

Used for storing temporary files.

## **`/usr`**

Typically a **shareable, read-only directory**. Contains user applications andsupporting files for those applications. 

- `/usr/X11R6` is used by the X  Window System. 
- `/usr/bin` contains user accessible commands.
-  `/usr/doc` holds documentation for `/usr`
applications. 
- `/usr/include` this directory contains header files
   for the C compiler.
- `/usr/include/g++` contains header files for the
C++ compiler. 
- `/usr/lib` libraries, binaries, and object files that
aren't usually executed directly by users. 
- `/usr/local` used for installing software locally that needs to be safe from being overwritten when system software updates occur. 
- `/usr/man` is where the manual pages are kept.  
- `/usr/share` is for read-only independent data files. 
- `/usr/src` is used for  storing source code of applications installed and kernel sources and headers

## **`/var`**

This directory contains **variable data** files such as logs `(/var/log)` mail `(/var/mail)`, and spools `(/var/spool)` among other things.