# Files and Directories

**File**: Named collection of related information recorded on secondary storage.
Files are in contiguous logical address space.

## File Structure

1. **None**
2. **Simple record structure**
   - Lines
   - Fixed Length
   - Variable Length
3. **Complex structures**
   - Formatted documents
   - Relocatable load file


All application programs must include code to understand their file formats/structures
All operating systems must support at least one file structure, of executable file, a binary file

## File Attributes

In **DOS**/**Windows**: stored in directory structure, as part of **directory entry** for a file <br>
In **Unix**/**Linux**: known as **inode** in Linux

   1. **Name**: Symbolic filename, kept in human-readable form
   2. **Type**: 
   3. **Location**: pointer to location of file on device
   4. **Size**
   5. **Protection**: Access control, e.g, who can read/write into file
   6. **Owner**
   7. **Timestamp of creation**
   8. **Timestamp of update**
   9. **Read/Write pointer value**


## Directory Entry

A file is represented in a directory by its directory entry.<br>

In **DOS**/**Windows** a directory entry consists of file name and its attributes. <br>
In **UNIX**/**Linux**, a directory entry consists of file name and inode number

File Name character max: 255<br>
**Inode** number is used to access file's **inode**.

## File Operations

1. Create (`create`)
   1. space must be found for file in FileSystem.
   2. an for new file must be made in directory.
2. Open (`open`)
   - This operation take filename, searches directory,copy directory entry in **open-file table**
   - This operation can also accept modes, like read-only,read-write
   - **Returns a pointer** to the entry in **open-file table**.
3. Write (`write`)
   - make a system call, specifying both filename and information to be written
   - system search for filename in directory
4. Read (`read`)
5. Reposition within file (`lseek`)
6. Delete (`unlink`)
7. Truncate(`create`)
8. Close (`close`)
