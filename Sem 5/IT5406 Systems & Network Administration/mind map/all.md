# Introduction to System & Network Administration

## Duties of a System Administrator

### Overview of Responsibilities

- System administrators are responsible for controlling access to systems and networks, ensuring that only authorized users can access sensitive information.

- They add and configure hardware components to maintain and enhance system performance.

- Automating tasks is a key duty, allowing for efficiency and consistency in system operations.

- Regular oversight of backups is crucial to prevent data loss and ensure recovery in case of failures.

### Additional Responsibilities

- System administrators monitor system performance and troubleshoot issues to maintain optimal operation.

- They maintain local documentation to provide clear guidelines and records of system configurations and procedures.

- Vigilant security monitoring is essential to protect systems from unauthorized access and potential threats.

- Tuning performance involves adjusting system settings and configurations to improve efficiency and speed.

## Introduction to Linux Systems

### Understanding Linux Distributions

- A Linux distribution consists of the Linux kernel and various packages that provide commands and functionalities for the operating system.

- While all distributions share the same kernel lineage, they differ in format, type, and the number of packages included.

- Distributions vary in focus, support, and popularity, catering to different user needs and environments.

### Popular Linux Distributions

- Some widely used Linux distributions include:

	- Arch

	- CentOS

	- Debian

	- Fedora

	- Ubuntu

- Each distribution has its unique features and target audiences, from general users to enterprise environments.

## Man Pages and Other Online Documentation

### Importance of Man Pages

- Man pages, or manual pages, provide concise documentation for commands, drivers, and library routines in Linux.

- They are typically installed alongside software packages and serve as a primary resource for users to understand command usage and options.

- To access a man page, users can type the command  man <command>  in the terminal.

### Structure of Man Pages

- Man pages are organized into sections, including:

	- User-level commands and applications

	- System calls and kernel error codes

	- Library calls and device drivers

	- Miscellaneous files and documents

- This structured approach allows users to quickly find relevant information based on their needs.

## Ways to Find and Install Software

### Finding Available Packages

- To check if a package is already installed, users can utilize the  which  command to locate binaries in their search path.

- For example, typing  which <application/package name>  will reveal if the application is available on the system.

### Installing New Software

- Software can be installed using package managers like  apt  or  yum , which simplify the process of obtaining and managing software.

- Alternatively, users can build software from source code by downloading it, compiling it, and installing it manually.

- Some applications can also be installed via web scripts that automate the download and installation process.

## Specialization and Adjacent Disciplines

### Overlapping Roles

- System administrators often work alongside other specialists, including:

	- DevOps professionals who integrate development and operations.

	- Site reliability engineers focused on system uptime and reliability.

	- Security operations engineers who ensure system security.

	- Network and database administrators managing specific system components.

### Importance of Collaboration

- Collaboration among these roles is essential for building and maintaining complex networks effectively.

- Each role contributes unique skills and perspectives, enhancing the overall performance and security of the IT infrastructure.

## Ethics and Code of Conduct

### Ethical Responsibilities

- System administrators must uphold professionalism and personal integrity in their work.

- They are responsible for maintaining privacy and adhering to laws and policies related to information technology.

- Effective communication is vital for conveying technical information clearly to diverse audiences.

### Commitment to the Community

- System administrators have a responsibility to the computing community, ensuring that their actions contribute positively to the field.

- They must also consider social and ethical responsibilities, promoting best practices and ethical behavior in technology use.

### Reference for Ethical Guidelines

- The ethical guidelines for system administrators can be found in resources such as the LOPSA Code of Ethics, which outlines the principles and responsibilities expected of IT professionals.

# Installing an Operating System

## The Boot Process and Boot Loaders

### Definition and Overview of Boot Process

- The boot process is the sequence of events that occurs when a computer is powered on, leading to the loading of the operating system.

- Boot loaders are essential components that identify and load the operating system kernel into memory.

- The boot process involves several stages, including hardware probing, boot device selection, and kernel loading.

### Steps in the Linux Boot Process

- The process begins with the BIOS or UEFI loading from NVRAM upon power-on.

- The system probes for hardware and selects the boot device, which could be a disk or network.

- The boot loader, such as GRUB, is loaded, which then determines which kernel to boot and initiates the loading of the kernel.

### BIOS vs. UEFI

- BIOS (Basic Input/Output System) is the traditional firmware interface that uses the MBR (Master Boot Record) for booting.

- UEFI (Unified Extensible Firmware Interface) is a modern replacement for BIOS that supports GPT (GUID Partition Table) for more advanced disk partitioning.

- UEFI provides faster boot times and enhanced security features compared to traditional BIOS.

## The Grand Unified Boot Loader (GRUB)

### Overview of GRUB

- GRUB is the default boot loader for most Linux distributions, developed by the GNU project.

- It allows for the configuration of boot options and kernel parameters through a configuration file named grub.cfg.

- The configuration file is typically located in /boot/grub or /boot/grub2, with the main settings found in /etc/default/grub.

### Common GRUB Configuration Options

- GRUB_BACKGROUND: Specifies the background image for the boot menu.

- GRUB_DEFAULT: Sets the default menu entry to boot.

- GRUB_TIMEOUT: Defines the time in seconds to display the boot menu before automatically booting the default entry.

- GRUB_DISABLE_RECOVERY: Prevents the generation of recovery mode entries.

### GRUB Command Line Interface

- GRUB provides a command-line interface for users to edit boot entries at runtime.

- Key commands include:

	- boot: Boots the system from the specified kernel image.

	- linux: Loads a specified Linux kernel.

	- reboot: Reboots the system.

	- search: Searches for devices by file, filesystem label, or UUID.

## System Management Daemons

### Role of Init and System Management

- The init process, which has PID 1, is responsible for starting system processes and managing services.

- It performs essential tasks such as setting the computer name, configuring network interfaces, and starting other daemons.

- Init runs scripts and commands designed for specific contexts, ensuring the system operates smoothly.

### Transition from Init to Systemd

- Systemd has replaced traditional init systems, formalizing and enhancing process management.

- It allows for parallel management of processes, network connections, and logging.

- Systemctl is the command used to investigate and modify systemd configurations.

### Responsibilities of System Management Daemons

- System management daemons handle background tasks, ensuring that necessary services are running.

- They manage system resources, monitor system health, and respond to system events.

- These daemons are essential for maintaining system stability and performance.

## Reboot and Shutdown Procedure

### Commands for Shutting Down Systems

- The halt command is used to shut down the system safely, logging the shutdown and killing non-essential processes.

- The reboot command performs similar functions but restarts the system instead of halting it.

- The shutdown command provides a higher-level interface for scheduling shutdowns and notifying users.

### Importance of Proper Shutdown Procedures

- Proper shutdown procedures prevent data loss and corruption by ensuring all processes are terminated gracefully.

- They help maintain system integrity by flushing cached filesystem blocks to disk before halting the kernel.

- Scheduled shutdowns can be communicated to users, allowing them to save their work.

## Stratagems for a Non-Booting System

### Approaches to Troubleshooting Boot Issues

- When a system fails to boot, administrators can restore it to a known-good state without debugging.

- Alternatively, they can boot the system minimally to access a shell for interactive debugging.

- Another method involves booting from a separate system image to investigate the problematic system's filesystems.

### Common Causes of Boot Failures

- Boot failures can arise from hardware malfunctions, corrupted boot loaders, or misconfigured system files.

- Understanding the boot process helps in diagnosing issues effectively.

- Regular maintenance and updates can prevent many common boot problems.

## Drivers and the Kernel

### Role of the Kernel in System Management

- The kernel abstracts the complexity of hardware interactions, providing a stable API for application programmers.

- It manages hardware devices, processes, memory, and I/O facilities, ensuring efficient operation of the system.

- The kernel also handles housekeeping functions such as startup, shutdown, and multitasking.

### Understanding Device Drivers

- Device drivers act as an interface between the kernel and hardware devices, translating commands for specific hardware.

- They allow the kernel to communicate with various hardware components without needing to understand their specifics.

- Properly functioning drivers are crucial for system stability and performance, as they ensure hardware operates correctly within the system.

# Host Management in Linux

## Overview of Host Management

### Introduction to Host Management

- Host management encompasses various essential topics such as user management, process management, access control, software installation management, logging, storage, and file system management.

- Understanding these components is crucial for effective systems and network administration in a Linux environment.

### Intended Learning Outcomes

- By the end of this lesson, learners will be able to:

	- Install software using the Linux package management system.

	- Implement user management practices in a Linux distribution.

	- Explain various storage technologies.

	- Demonstrate user access control mechanisms.

	- Manage file system access control.

	- Execute process management tasks in a Linux environment.

## Access Control and Rootly Powers

### Standard UNIX Access Control

- Access control decisions are based on the user attempting an operation or their membership in a UNIX group.

- Each object (files, processes) has an owner who has control over it, and the special user account "root" can act as the owner of any object.

- Only the root user can perform sensitive administrative operations, such as creating device files and configuring network interfaces.

### File System Access Control

- The kernel and filesystem are closely linked, controlling devices through files in  /dev .

- Every file has an owner and a group, with permissions set by the owner.

- User Identification Number (UID) and Group Identification Number (GID) are used to track ownership.

### Process Ownership and Management

- The owner of a process can send signals and adjust the process's scheduling priority.

- Processes have multiple identities: real, effective, and saved UID/GID.

- The root account is the administrative user with the highest privileges, capable of performing critical system tasks.

### Management of Root Account

- Direct root login should be disabled to enhance security.

- The  su  command allows users to switch to the root account, while  sudo  provides limited root access with logging capabilities.

- The  /etc/sudoers  file defines who can use  sudo  and what commands they can execute.

## Process Control

### Components of a Process

- Each process has a unique Process ID (PID), Parent PID (PPID), and user/group IDs.

- The process's state can be runnable, sleeping, or stopped, influencing how it interacts with system resources.

### The Life Cycle of a Process

- A new process is created using the  fork  system call, often followed by an  exec  call to run a new program.

- The  init  or  systemd  process is crucial for managing system processes.

- Parent processes must acknowledge the termination of child processes using the  wait  system call.

### Monitoring Processes

- The  ps  command is used to monitor active processes, while  top  provides interactive monitoring.

- Commands like  nice  and  renice  adjust process scheduling priorities.

- The  /proc  filesystem contains information about running processes.

### Runaway Processes

- Runaway processes consume excessive system resources, identifiable through  ps  or  top  outputs.

- Monitoring system load averages helps determine if the system is overloaded.

- Tools like  strace  can trace system calls made by processes to diagnose issues.

## Software Installation and Management

### Managing Packages in Linux

- Linux software is distributed as packages, which include binaries, dependencies, and configuration files.

- Common package formats include RPM (used in Red Hat-based systems) and DEB (used in Debian-based systems).

### High-Level Linux Package Management Systems

- APT (Advanced Package Tool) and YUM (Yellowdog Updater, Modified) are popular package management systems.

- APT commands include  apt-get  for installing and updating packages, while YUM automates dependency resolution.

### Software Localization and Configuration

- Proper organization of software localization is essential for managing multiple devices with different configurations.

- Regular updates and testing of configurations are critical for maintaining system security and functionality.

## User Management

### User Accounts and the /etc/passwd File

- User accounts are identified by User ID (UID), with the  /etc/passwd  file containing user details.

- Each line in  /etc/passwd  includes the login name, encrypted password placeholder, UID, GID, home directory, and login shell.

### The /etc/shadow File

- The  /etc/shadow  file stores encrypted passwords and additional account information, accessible only by the superuser.

- It includes details such as the date of the last password change and password expiration policies.

### Adding and Removing Users

- User accounts can be added manually by editing the  /etc/passwd  and  /etc/group  files or using commands like  useradd .

- Removing users involves cleaning up associated files and processes, ensuring no remnants remain in the system.

### User Login Lockout and PAM

- User accounts can be locked using the  usermod  command, enhancing security.

- Pluggable Authentication Modules (PAM) centralize authentication management, allowing for various methods beyond passwords.

## Logging

### Log Management

- Log management involves collecting logs from various sources and providing structured interfaces for querying and analyzing messages.

- Most log files are located in the  /var/log  directory, while systemd uses the  journalctl  command for log management.

### The System Journal

- The systemd journal collects messages from multiple sources, including the kernel and user applications.

- The journal stores messages in a binary format, allowing for efficient searching and indexing.

### Syslog and Kernel Logging

- Syslog provides a standardized logging protocol, capturing essential information such as timestamps and process names.

- Kernel logs can be accessed using the  dmesg  command, which displays boot-time activities and kernel messages.

### Log Rotation and Management Strategies

- The  logrotate  tool manages log files, ensuring they do not consume excessive disk space.

- Organizations should establish logging policies that define retention periods, types of events to log, and access controls for log data.

## Storage Management

### Storage Hardware and Interfaces

- Understanding different types of storage hardware (HDDs, SSDs) and their interfaces (SATA, PCIe) is crucial for effective storage management.

- Tools like  lsblk  and  parted  help manage and monitor disk partitions and configurations.

### Disk Partitioning and Logical Volume Management

- Proper disk partitioning enhances system performance and organization, with guidelines for separating critical filesystems.

- Logical Volume Management (LVM) allows for flexible disk management, enabling dynamic resizing and snapshots of volumes.

### Redundant Arrays of Inexpensive Disks (RAID)

- RAID improves performance and data redundancy, with various levels (0, 1, 5, 6) offering different trade-offs between speed and data protection.

- Software RAID can be managed using tools like  mdadm , allowing for easy configuration and monitoring.

### Next Generation File Systems

- Newer file systems like ZFS and BTRFS offer advanced features such as snapshots, error detection, and improved performance.

- These file systems provide robust solutions for modern storage needs, including data integrity and efficient management of storage pools.

### Data Backup Strategies

- Organizations must develop comprehensive data backup strategies to protect against data loss due to hardware failure, security breaches, or corruption.

- Backup plans should include timelines for regular backups, validation processes, and access controls to ensure data security and integrity.

# Networking Administration

## Overview of Networking Administration

### Introduction to Key Topics

- This section covers essential topics related to Linux networking, including the domain name system (DNS), single sign-on (SSO), and web hosting.

- Understanding these components is crucial for effective systems and network administration.

- Each topic will be explored to provide a comprehensive understanding of its significance in network management.

## Intended Learning Outcomes

### Goals for Students

- By the end of this lesson, students will be able to:

	- Configure and troubleshoot networks using Linux.

	- Deploy and manage a domain name system.

	- Explain the concept of Single Sign-On and its implementations.

	- Configure and implement web hosting solutions.

## Networking in Linux

### Methods for Configuring Networks

- There are several methods to configure networks in Linux systems:

	- Using command-line tools such as  ip  or  ifconfig .

	- Utilizing NetworkManager, which can operate with a graphical user interface (GUI) or command-line interface (CLI).

	- Editing configuration files directly for network settings.

- After making configuration changes, it is advisable to reboot the system or restart the network service to apply the new settings.

### NetworkManager

- NetworkManager is a tool designed to manage network connections automatically.

- It can run in the background and assess available networks, prioritizing wired connections over wireless ones.

- Users can manage NetworkManager rather than relying solely on system administrators.

### Command-Line Tools

- Key command-line tools for network configuration include:

	-  ifconfig : Used to configure network interfaces.

	-  ip : A more modern tool for network management.

- These tools provide essential functionalities for network setup and troubleshooting.

### Configuration Files

- Different Linux distributions have specific configuration files for network settings.

- For example, in CentOS, network configuration files are located in the  /etc/sysconfig/network-scripts/  directory.

- Editing the relevant interface configuration file (e.g.,  ifcfg-enp0s3 ) is necessary for network adjustments.

## Network Troubleshooting

### Basic Troubleshooting Tools

- Several tools are available for troubleshooting network issues in Linux:

	- Ping: Checks if a host is reachable.

	- Traceroute: Identifies the path packets take to reach a destination.

	- Tcpdump: Captures network traffic for analysis.

	- Netstat: Displays network connections and statistics.

### Using Ping

- The  ping  command is a fundamental tool for verifying the availability of a network host.

- It sends ICMP echo requests and listens for replies, helping diagnose connectivity issues.

### Traceroute Functionality

- The  traceroute  command helps trace the route packets take to a specified destination.

- It can reveal the gateways and hops along the path, assisting in identifying where delays or failures occur.

### Tcpdump for Traffic Analysis

-  tcpdump  is a powerful command-line packet analyzer that captures network traffic.

- It allows administrators to inspect packets flowing through network interfaces, aiding in diagnosing complex network issues.

## Network Monitoring

### Importance of Network Monitoring Tools

- Network monitoring tools provide insights into system performance and network health.

- They collect data from various sources to summarize ongoing trends and alert administrators to potential problems.

- Examples of monitoring tools include:

	- SmokePing: Monitors network latency.

	- iPerf: Measures bandwidth and performance.

	- Cacti: Provides graphical representation of network data.

## Firewalls and NAT

### Understanding iptables

-  iptables  is a user-space utility for configuring the Linux kernel firewall.

- It applies ordered chains of rules to network packets, allowing for packet filtering and network address translation (NAT).

- The default table for filtering is the "filter" table, which includes three chains: FORWARD, INPUT, and OUTPUT.

### Configuring iptables

- To use  iptables  effectively, administrators must enable IP forwarding and load necessary kernel modules.

- A typical firewall setup involves a series of  iptables  commands executed in a startup script.

### Implementing NAT

- NAT allows local hosts to access the Internet while hiding their internal IP addresses.

- To enable NAT, administrators must modify kernel variables and use  iptables  commands to route packets appropriately.

## The Domain Name System (DNS)

### DNS Architecture

- DNS is a distributed hierarchical database essential for name resolution on the Internet.

- It consists of various servers, including authoritative and caching servers, which handle queries and responses.

### Configuring DNS in Linux

- Linux systems can be configured to resolve domain names using files such as  resolv.conf  and  nsswitch.conf .

- The  /etc/hosts  file can also be used for local name resolution.

### Understanding DNS Resource Records

- DNS uses resource records (RR) to store information about domain names, including:

	- A records: Map hostnames to IPv4 addresses.

	- AAAA records: Map hostnames to IPv6 addresses.

	- MX records: Define mail exchange servers for a domain.

## Single Sign-On (SSO)

### Core Elements of SSO

- SSO involves a centralized directory store for managing user information and authenticating identities.

- It simplifies user access across multiple applications by allowing a single set of credentials.

### LDAP Service in SSO

- The Lightweight Directory Access Protocol (LDAP) serves as a central repository for user attributes and account information.

- It supports various applications in authenticating users without managing account details directly.

### Implementing Directory Services

- Students are encouraged to implement and deploy directory services, configuring  sssd  and  pam  for user authentication through LDAP.

## Web Hosting

### Understanding HTTP

- HTTP (Hypertext Transfer Protocol) is a client/server protocol used for transferring data on the web.

- It has evolved from plain text in HTTP/1.0 and 1.1 to a binary format in HTTP/2 for improved efficiency.

### Structure of HTTP Transactions

- An HTTP transaction consists of requests and responses, with headers providing metadata about the data being transferred.

- Students should familiarize themselves with tools like  curl  for testing HTTP interactions.

### Web Server Basics

- Web servers play a crucial role in serving content and managing HTTP requests.

- They can handle static content, proxy requests to application servers, and implement features like virtual hosting and TLS connections.

### Load Balancing and Caching

- Load balancers distribute incoming requests across multiple servers to prevent overload and ensure high availability.

- Caching mechanisms store frequently requested data to improve response times and reduce server load.

### Apache and NGINX Configuration

- Apache and NGINX are popular web server software, each with unique configuration requirements for hosting websites.

- Understanding how to configure these servers for virtual hosting, TLS, and load balancing is essential for effective web hosting management.
# Automating System Administration

## Overview of Automating System Administration

### Introduction to Automation in System Administration

- Automation in system administration involves using scripts and tools to streamline repetitive tasks, enhancing efficiency and reducing human error.

- The course covers various scripting languages and tools, emphasizing their application in daily administrative tasks.

- Key topics include shell scripting, Python scripting, and version control with Git, which are essential for modern system administrators.

## Scripting Philosophy

### Principles of Effective Scripting

- Writing microscripts is encouraged to simplify daily tasks and improve productivity.

- Familiarity with essential tools such as shell and text editors is crucial for effective scripting.

- Emphasizes the importance of not optimizing prematurely and selecting the appropriate scripting language for specific tasks.

- Following best practices in scripting ensures maintainability and readability of code.

## Shell Basics

### Understanding Shells and Commands

- Linux systems feature various shell programs, including Bourne shell (sh), Almquist shell (ash), Bourne-again shell (bash), Korn shell (ksh), and C shell (csh).

- Bash is the most widely used shell and serves as the standard for scripting.

- Basic shell commands include man, ls, mkdir, cp, mv, which are fundamental for navigating and managing files in a Linux environment.

### Working with Shell Commands

- Knowledge of pipes and redirection is essential for effective command-line operations.

- Environment variables play a significant role in configuring the shell environment.

- Filter commands such as grep, sort, head, tail, and tee are vital for processing and manipulating text data.

## Shell Scripting

### Creating and Executing Shell Scripts

- A shell script can consist solely of command lines, with the first line known as the "shebang" indicating the script interpreter (e.g., /bin/bash).

- Proper execution and read permissions are necessary to run a script successfully.

- User input can be read within scripts, allowing for dynamic execution based on user parameters.

### Control Structures in Shell Scripting

- Conditions in shell scripts enable decision-making processes, allowing scripts to execute different commands based on specific criteria.

- Loops, including for and while loops, are fundamental for iterating over data or executing commands multiple times.

- Arithmetic operations can be performed within scripts, enhancing their functionality and allowing for complex calculations.

## Regular Expressions

### Utilizing Regular Expressions in Scripting

- Regular expressions are standardized patterns used for parsing and manipulating text, crucial for data validation and extraction.

- The comparison operator =~ is used to match patterns within strings, facilitating text processing.

- Common patterns include:

	- [0-9] for any single digit.

	- [A-Z] for any capital letter.

	- ^ for the beginning of a string and $ for the end of a string.

## Python Scripting

### Introduction to Python for System Administration

- Python is an interpreted, general-purpose scripting language known for its extensive libraries and ease of use.

- It is widely adopted for system administration tasks due to its versatility and powerful features.

- Python 2 and Python 3 are the two primary versions, with Python 3 being the recommended version for new projects.

### Writing Python Scripts

- Simple Python scripts can automate tasks and enhance productivity in system administration.

- Familiarity with Python's syntax and libraries is beneficial for effective scripting and automation.

- Python's readability and community support make it an ideal choice for both beginners and experienced developers.

## Version Control with Git

### Importance of Revision Control

- Keeping track of configuration and code changes is vital for troubleshooting and maintaining system integrity.

- Revision control systems like Git provide an organized way to manage file modifications, allowing for easy recovery of previous versions.

- Git facilitates collaboration among multiple editors, preventing conflicts and ensuring that changes are integrated smoothly.

### Basic Git Commands

- git init: Initializes a new Git repository by creating the necessary .git directory.

- git add: Stages changes from the working directory for the next commit, preparing them for versioning.

- git commit: Records the staged changes into the repository, creating a snapshot of the project at that point in time.

## References

### Evi Nemeth, Garth Snyder, Trent R. Hein, Ben Whaley, and Dan Mackin. "UNIX and Linux System Administration Handbook" (5th Edition), Pearson Education, Inc., 2018.



# Virtualization and Cloud Computing

## Cloud Computing

### Definition and Overview

- Cloud computing is the practice of leasing computer resources from a pool of shared capacity.

- Users provision resources on demand and pay a metered rate for consumption.

- The transition from private data centers to cloud services has been rapid and transformative.

- Cloud providers create advanced infrastructure designed for energy efficiency and minimal maintenance.

### Factors Influencing Cloud Provider Choice

- Cost is a primary consideration when selecting a cloud provider.

- Past experience with a provider can influence future decisions.

- Compatibility with existing technology is crucial for seamless integration.

- Security and compliance requirements must be met to protect data and adhere to regulations.

- Internal politics may also play a role in the decision-making process.

### Cloud Platform Choices

- There are three main categories of cloud services:

	- Infrastructure-as-a-Service (IaaS) provides virtualized computing resources over the internet.

	- Platform-as-a-Service (PaaS) offers hardware and software tools over the internet, typically for application development.

	- Software-as-a-Service (SaaS) delivers software applications over the internet on a subscription basis.

### Cloud Service Fundamentals

- Most cloud providers use a web-based GUI as the primary interface for users.

- Data centers are maintained globally, organized into regions and availability zones.

- Virtual private servers (VPS) are instances that run on the provider's hardware.

- Networking capabilities allow the creation of virtual networks with custom topologies.

- Cloud providers offer advanced storage systems, identity and authorization features, and automation tools.

- Serverless functions allow code execution without the need for long-lived infrastructure.

### Major Public Cloud Providers

- Prominent public cloud providers include:

	- Amazon Web Services (AWS)

	- Google Cloud Platform (GCP)

	- DigitalOcean (DO)

### Cost Control in Cloud Services

- Pricing for cloud services is based on various factors:

	- Compute resources are billed per hour of use.

	- Internet data transfer is charged per GiB or TiB.

	- Storage costs are calculated per GiB or TiB stored monthly.

- Customers are encouraged to design methods to minimize cloud service costs.

## Virtualization

### Definition and Overview

- Virtualization involves using software or hardware to mediate between virtual machines (VMs) and the underlying hardware.

- Hypervisors manage system resources among guest operating systems, which are isolated from one another.

- Guest operating systems operate independently, enhancing security and resource management.

### Types of Hypervisors

- Hypervisors can be categorized into:

	- Full virtualization, which provides complete abstraction of the hardware.

	- Paravirtualization, which requires guest OS modifications for better performance.

	- Hardware-assisted virtualization, which leverages CPU features to improve efficiency.

	- Paravirtualized drivers, which enhance communication between the guest OS and the hypervisor.

### Type 1 vs. Type 2 Hypervisors

- Type 1 hypervisors run directly on the hardware, providing better performance and efficiency.

- Type 2 hypervisors run on top of a host operating system, making them easier to set up but less efficient.

### Live Migration and Virtual Machine Images

- Live migration allows VMs to move between hypervisors without service interruptions.

- Virtual machine images are templates of configured operating systems that hypervisors can load and execute.

### Containerization

- Containerization is a form of OS-level virtualization that isolates processes without using a hypervisor.

- It relies on kernel features to provide lightweight and efficient resource management.

### Open Source Virtualization Projects

- Leading open-source virtualization projects include:

	- Xen, a paravirtual hypervisor that powers major public clouds.

	- KVM (Kernel-based Virtual Machine), integrated into the Linux kernel, providing full virtualization.

## Containers

### Background and Core Concepts

- Containers utilize kernel support features such as namespaces, control groups, and capabilities for isolation.

- Docker has emerged as a leading container engine, relying on these kernel features for efficient container management.

### The Open Source Container Engine – Docker

- Docker provides a platform for developing, shipping, and running applications in containers.

- It simplifies the deployment process and enhances application scalability and portability.

### Container Management and Networking

- Container management systems offer features for orchestrating and managing containerized applications.

- Networking capabilities allow containers to communicate with each other and external systems securely.

### Containers in Practice

- Best practices for working with containers include:

	- Using the host's cron daemon for scheduling tasks.

	- Avoiding SSH within containers; instead, use docker exec for interactive sessions.

	- Configuring applications to accept settings from environment variables.

### Security and Logging in Containers

- Security measures include restricting access to the Docker daemon, using TLS, and running processes as unprivileged users.

- Logging practices should be established to monitor container activity and troubleshoot issues effectively.

### Container Clustering and Management

- Container management systems include:

	- Kubernetes, a powerful orchestration tool for managing containerized applications.

	- Docker Swarm, which provides native clustering for Docker containers.

	- AWS EC2 Container Service, which integrates with Amazon's cloud infrastructure for container management.

