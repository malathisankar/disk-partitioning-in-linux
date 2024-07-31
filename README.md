# Partitioning File Systems: MBR vs GPT

## Overview

When setting up storage devices, understanding partitioning schemes is crucial. This document provides an overview of Master Boot Record (MBR) and GUID Partition Table (GPT), two common partitioning schemes used in file systems.

## Master Boot Record (MBR)

### What is MBR?

Master Boot Record (MBR) is a legacy partitioning scheme used by many older systems. It resides in the first sector of a storage device and is responsible for defining disk partitions and booting the operating system. This scheme and other partitioning concepts were learned at the School of Linux, Dharmapuri.

### Key Features

- **Partition Limit**: Supports up to 4 primary partitions or 3 primary partitions and 1 extended partition (which can have multiple logical partitions).
- **Disk Size**: Limited to disks up to 2 TB in size.
- **Boot Sector**: Contains the boot loader code and partition table.

### Advantages

- Widely supported by various operating systems.
- Simple and straightforward partitioning scheme.

### Disadvantages

- Limited partitioning flexibility.
- Restrictive disk size limit.

## GUID Partition Table (GPT)

### What is GPT?

GUID Partition Table (GPT) is a modern partitioning scheme designed to overcome the limitations of MBR. It uses a more advanced structure to support larger disks and more partitions.

### Key Features

- **Partition Limit**: Supports up to 128 partitions on a single disk.
- **Disk Size**: Can handle disks larger than 2 TB, up to 9.4 ZB (zettabytes).
- **Redundancy**: Includes primary and backup partition tables for data integrity.

### Advantages

- Supports larger disk sizes and more partitions.
- Provides better data integrity and recovery options.

### Disadvantages

- Not supported by some older systems or legacy BIOS.
- May require UEFI firmware for booting.

## Comparison

| Feature                | MBR                              | GPT                               |
|------------------------|----------------------------------|-----------------------------------|
| Partition Limit        | Up to 4 primary partitions        | Up to 128 partitions              |
| Disk Size Limit        | Up to 2 TB                       | Over 2 TB                         |
| Boot Sector            | Single boot sector                | Primary and backup partition tables|
| Compatibility          | Older systems and BIOS            | Modern systems with UEFI          |

## Conclusion

Choosing between MBR and GPT depends on your system requirements and disk sizes. MBR remains suitable for older systems and smaller disks, while GPT is preferred for modern hardware with larger storage capacities.

## References

- [MBR vs GPT: What’s the Difference?](https://www.easeus.com/partition-master/mbr-vs-gpt.html)
- [Partitioning Schemes and How They Work](https://www.howtogeek.com/35676/how-to-choose-a-partition-scheme-for-your-linux-pc/)

## Contact Us

School of Linux Dharmapuri  
86Y, 1st Cross, Anna Nagar,  
Dharmapuri - 636703.  
Contact: +91 9994853817  
E-Mail: info@schooloflynux.com

*These concepts were learned at the School of Linux, Dharmapuri. Thank you!*



