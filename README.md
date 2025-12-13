# Storage-for-DevOps-Engineers

**_1.What types of storage are there?_**

- File
- Block
- Object

**_2.Explain Object Storage_**

- Data is divided to self-contained objects
- Objects can contain metadata

**_3.What are the pros and cons of object storage?_**

- Pros:
  - Usually with object storage, you pay for what you use as opposed to other storage types where you pay for the storage space you allocate
  - Scalable storage: Object storage mostly based on a model where what you use, is what you get and you can add storage as need 

- Cons:
  - Usually performs slower than other types of storage
  - No granular modification: to change an object, you have re-create it
 
**_4.What are some use cases for using object storage?_**

- Backup and Restore: Storing application and database backups for disaster recovery and long-term retention.

- Archiving: Moving infrequently accessed or regulatory-required data (e.g., logs, historical snapshots) to cost-effective, durable storage.

- Static Website Hosting: Directly hosting files (HTML, CSS, JavaScript, images) for high-availability, low-cost static websites.
  
- CI/CD Artifacts: Storing build artifacts (e.g., JARs, Docker images, executables) created by Continuous Integration pipelines.

- Log Data Lake: Centralizing massive volumes of application, system, and security logs for analysis and compliance.

- Big Data Storage: Providing the durable, scalable backbone for large datasets used by analytics and machine learning tools (e.g., in a Hadoop/Spark environment).

**_5.Explain File Storage_**

- File Storage used for storing data in files, in a hierarchical structure
- Some of the devices for file storage: hard drive, flash drive, cloud-based file storage
- Files usually organized in directories

**_6.What are the pros and cons of File Storage?_**

- Pros
  - 1.Familiar Interface: Uses a standard, intuitive folder and file hierarchy structure.
  - 2.Shared Access/Locking: Easily supports concurrent access and file locking (via protocols like NFS/SMB) critical for collaboration.
  - 3.Low Latency for Small Files: Offers good performance for frequent read/write operations on smaller, structured files.

- Cons
  - 1.Limited Scalability: Becomes difficult and expensive to scale to petabyte capacity; performance degrades with millions of files in a single structure.
  - 2.Management Overhead: Hierarchical structure requires manual capacity planning and management of file paths, quotas, and permissions.
  - 3.Basic Metadata: Only supports limited, basic metadata (name, date, size), hindering advanced searching and analytics compared to object storage.
 
**_7.What are some examples of file storage?_**

- Local filesystem
- Dropbox 
- Google Drive

**_8.What types of storage devices are there?_**

- 1. Primary Storage (Memory)
- Directly accessible by the CPU; very fast but usually smaller.
  - RAM (Random Access Memory): Volatile (data lost when power off). Used for currently executing programs and active data.
  - ROM (Read-Only Memory): Non-Volatile. Stores firmware (like BIOS) needed to boot the computer.

- 2. Secondary Storage (Mass Storage)
- Non-volatile, high capacity, and slower than primary storage. Used for long-term retention of operating systems, applications, and user files.
  - Magnetic: Hard Disk Drives (HDDs), Magnetic Tape.
  - Flash/Solid-State: Solid-State Drives (SSDs), USB Flash Drives, SD Cards.
  - Optical: CDs, DVDs, Blu-ray Discs.

- 3. Storage Architectures (DevOps/Enterprise Focus)
  - Block Storage: Data stored as fixed-size blocks (e.g., in a SAN or for virtual machine disks).
  - File Storage: Data stored in a hierarchical directory structure (e.g., NAS, shared drives).
  - Object Storage: Data stored as discrete objects in a flat structure, accessed via APIs (e.g., Amazon S3, Azure Blob Storage).
 
**_9.Explain IOS_**

- IOPS measures the number of individual read and write operations a storage device (HDD, SSD, SAN) can perform per second.

**_10.Explain storage throughput_**

- Storage throughput (or data transfer rate) measures the total volume of data transferred to or from a storage device per second.
- Typically measured in Megabytes per second (MB/s) or Gigabytes per second (GB/s).

**_11.What is a filesystem?_**

- A file system is a way for computers and other electronic devices to organize and store data files. It provides a structure that helps to organize data into files and directories, making it easier to find and manage information.
- A file system is crucial for providing a way to store and manage data in an organized manner.

- Commonly used filed systems: 
  - Windows:
    - NTFS
    - exFAT
  - Mac OS:
    - HFS+ *APFS
      
**_12.Explain Dark Data._**

- Information assets collected and stored by organizations during regular activities, but which are not actively used for analytics, decision-making, or monetization.

- Examples
  - Server/System Logs: Logs that are collected but never analyzed for performance bottlenecks or security threats.
  - IoT Sensor Data: Raw telemetry data from devices that is stored but ignored.
  - Old Email Archives: Forgotten conversations potentially containing key decisions or customer feedback.
  - Chat Logs/Call Transcripts: Customer support or internal communications that are not mined for insights.
  - Obsolete Backups/Archives: Data kept long after its business purpose or regulatory mandate has passed.
 
- Risks:
  - Compliance: May contain sensitive data subject to regulations without proper governance.
  - Cost: Incurs unnecessary storage and maintenance expenses.
  - Security: Represents a potential attack surface if unencrypted and forgotten.
 
- Oppurtunity: Contains valuable, untapped insights into operational efficiency, customer behavior, and security vulnerabilities.

**_13.Explain MBR_**

- A special type of boot sector located at the very beginning of a partitioned storage device (like a HDD or SSD).

- To hold the information about the drive's partitions and act as a loader for the operating system.
