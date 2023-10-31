# What is an Operating System?

An operating system (OS) is system software that manages computer hardware and provides various services for computer programs. It serves as an intermediary between the hardware and the user/application software, ensuring that the hardware resources are used efficiently and that users can interact with the computer in a more user-friendly and organized manner.

## Examples of popular operating systems include:

1. **Microsoft Windows:** Various versions of the Windows OS, such as Windows 10 and Windows 11, are widely used on personal computers and laptops.

2. **macOS:** Developed by Apple Inc., macOS is the operating system used on Apple Macintosh computers.

3. **Linux:** Linux is an open-source operating system kernel that serves as the basis for many Linux distributions (distros) like Ubuntu, Fedora, and CentOS. Linux is used on a wide range of devices, including servers, desktop computers, and embedded systems.

4. **Android:** Android is a mobile operating system developed by Google and is used on a vast number of smartphones and tablets.

5. **iOS:** iOS is Apple's mobile operating system, exclusively used on iPhones, iPads, and iPods.

6. **Unix:** Unix is a family of operating systems that has influenced many modern OSs, including Linux. Variants of Unix are used in server environments and embedded systems.

7. **FreeBSD:** FreeBSD is a Unix-like operating system known for its stability and is often used in server and networking environments.

8. **Windows Server:** Microsoft offers specialized versions of the Windows operating system for server environments, such as Windows Server 2019.

9. **IBM z/OS:** This is the mainframe operating system developed by IBM for their zSeries mainframe computers.

10. **RTOS (Real-Time Operating Systems):** Examples of RTOS include VxWorks and QNX, which are used in embedded systems and applications requiring real-time performance.

These are just a few examples of operating systems, and there are many more specialized and niche operating systems designed for various purposes and devices. The choice of an operating system depends on the specific requirements and intended use of the computer or device.

## The Linux Filesystem Hierarchy:

The Linux filesystem has a hierarchical structure:

1. **Root (/):** The top-level directory.
2. **Directories:** Folders to organize files.
3. **Files:** Data, programs, or links.
4. **Mount Points:** Devices integrated into the filesystem.
5. **File Permissions:** Control access to files.
6. **Pathnames:** Specify file locations.
7. **Hidden Files:** Start with a dot (.) and are often used for configuration.

Understanding this structure is vital for working with Linux.

# What is Shell?

Computers understand the language of 0's and 1's called binary language. In the early days of computing, instructions were provided using binary language, which is difficult for all of us to read and write. So in the OS, there is a special program called Shell. Shell accepts your instructions or commands in English and translates them into the computer's native binary language.

![Shell](https://github.com/janjiralakirankumar/Shell-Scripting-Guide/assets/137407373/7fcfb0f4-7620-4720-ab2a-7ffda277f4df)

## Types of Shells:

- **BASH (Bourne-Again Shell):** Developed by Brian Fox and Chet Ramey, it's the most common shell in Linux and is freeware.
- **CSH (C Shell):** Created by Bill Joy at the University of California for BSD. It has syntax similar to the C programming language.
- **KSH (Korn Shell):** Developed by David Korn at AT&T Bell Labs.
- **TCSH:** An enhanced and compatible version of the Berkeley UNIX C shell (CSH).

## Basic Linux Commands:

Here's a list of fundamental Linux commands with examples for each category:

### Manual:

- `man`: Display manual pages for commands. Example: `man ls`

### File Handling Commands:

- `ls`: List files and directories. Example: `ls`
- `pwd`: Print the current working directory. Example: `pwd`
- `cd`: Change the current directory. Example: `cd /home/user/documents`
- `touch`: Create an empty file. Example: `touch newfile.txt`
- `mkdir`: Create a new directory. Example: `mkdir new_directory`
- `rm`: To remove a file: `rm file.txt` / To remove an empty directory: `rmdir empty_directory`
- `cp`: Copy files and directories. Example: `cp file.txt /backup/`
- `mv`: To move a file: `mv file.txt new_location/` / To rename a file: `mv old_name.txt new_name.txt`
- `cat`: Display file contents. Example: `cat file.txt`
- `more`: View text files page by page. Example: `more largefile.txt`
- `less`: View text files page by page. Example: `less bigfile.txt`
- `head`: Display the beginning of a text file. Example: `head file.txt`
- `tail`: Display the end of a text file. Example: `tail logfile.txt`

### Text Processing:

- `grep`: Search text within files using regular expressions. Example: `grep "keyword" file.txt`
- `sed`: Stream editor for text manipulation. Example: `sed 's/old-text/new-text/g' file.txt`
- `awk`: Text processing tool for data extraction and reporting. Example: `awk '{print $1}' file.txt`

### Process Management:

- `ps`: List currently running processes. Example: `ps`
- `top`: Provide a dynamic view of system processes. Example: `top`
- `kill`: Terminate a process by sending a signal. Example: `kill -9 process_id`
- `pkill`: Terminate processes based on their names. Example: `pkill -f process_name`
- `pgrep`: List process IDs based on process names. Example: `pgrep -l process_name`

Feel free to copy and paste these commands into your Linux terminal to execute them. Replace specific arguments with your own values.
