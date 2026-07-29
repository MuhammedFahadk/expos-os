# Stage 2 – Understanding the Filesystem

**Date:** 29 July 2026

## Objective

Learn how the eXpFS filesystem stores files on the XSM disk and how to use the XFS Interface to manage them.

## Tasks Completed

- Formatted the XSM disk using the `fdisk` command.
- Created a sample data file and loaded it into the XSM disk using the XFS Interface.
- Examined the Disk Free List after formatting and after loading a file.
- Copied and inspected the Inode Table to locate the data block of the loaded file.
- Verified the Root File entry created for the loaded file.
- Exported the file back from the XSM disk to the Linux system.
- Completed the assignments by checking the Root File and observing the changes after deleting the file.

## What I Learned

- The XSM disk is organized using the eXpFS filesystem.
- The Disk Free List keeps track of used and free disk blocks.
- The Inode Table stores metadata such as file name, size, permissions, and data block numbers.
- The Root File provides file information that can be accessed from user programs.
- The XFS Interface acts as a bridge between the Linux system and the simulated XSM disk.

## Commands Used

```bash
./xfs-interface
fdisk
load --data sample.dat
copy
dump --inodeusertable
export
```

## Outcome

Successfully loaded, inspected, exported, and deleted files using the XFS Interface while understanding how eXpFS organizes file metadata and data blocks.