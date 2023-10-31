# What is an Operating System?

An operating system (OS) is system software that manages computer hardware and provides various services for computer programs. It serves as an intermediary between the hardware and the user/application software, ensuring that the hardware resources are used efficiently and that users can interact with the computer in a more user-friendly and organized manner.

## Examples of popular operating systems include:

![image](https://github.com/janjiralakirankumar/Shell-Scripting-Guide/assets/137407373/09fb24d9-59fd-4e77-b1c0-e8d8be2a5e7a)

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

Understanding this structure is vital for working with Linux.

![image](https://github.com/janjiralakirankumar/Shell-Scripting-Guide/assets/137407373/8a86c9e8-bf05-4a26-958a-6a07a13353c9)

1. **Root (/):** The top-level directory.
2. **Directories:** Folders to organize files.
3. **Files:** Data, programs, or links.
4. **File Permissions:** Control access to files.
5. **Pathnames:** Specify file locations.
6. **Hidden Files:** Start with a dot (.) and are often used for configuration.

# What is Shell?

Computers understand the language of 0's and 1's called binary language. In the early days of computing, instructions were provided using binary language, which is difficult for all of us to read and write. So in the OS, there is a special program called Shell. Shell accepts your instructions or commands in English and translates them into the computer's native binary language.

![Shell](https://github.com/janjiralakirankumar/Shell-Scripting-Guide/assets/137407373/7fcfb0f4-7620-4720-ab2a-7ffda277f4df)

## Types of Shells:

- **BASH (Bourne-Again Shell):** Developed by Brian Fox and Chet Ramey, it's the most common shell in Linux and is freeware.
- **CSH (C Shell):** Created by Bill Joy at the University of California for BSD. It has syntax similar to the C programming language.
- **KSH (Korn Shell):** Developed by David Korn at AT&T Bell Labs.
- **TCSH:** An enhanced and compatible version of the Berkeley UNIX C shell (CSH).

## Basic Linux Commands

**File Management:**

1. **Create a Directory (`mkdir`)**:
   - Command: `mkdir new_directory`
   - Explanation: Create a new directory with the specified name. For example:
   ```
   mkdir my_folder
   ```

2. **Create an Empty File (`touch`)**:
   - Command: `touch new_file.txt`
   - Explanation: Create an empty file with the specified name. For example:
   ```
   touch my_document.txt
   ```

3. **List Files and Directories (`ls`)**:
   - Command: `ls`
   - Explanation: List files and directories in the current directory. For example:
   ```
   ls
   ```

4. **Copy a File (`cp`)**:
   - Command: `cp source_file.txt destination_directory/`
   - Explanation: Copy a file to a specified destination directory. For example:
   ```
   cp my_file.txt /home/username/documents/
   ```

5. **Move or Rename a File (`mv`)**:
   - Command: `mv old_name.txt new_name.txt`
   - Explanation: Rename a file or move it to a different location. For example:
   ```
   mv my_old_file.txt my_new_file.txt
   ```

6. **Remove a File (`rm`)**:
   - Command: `rm file_to_delete.txt`
   - Explanation: Delete a file with the specified name. For example:
   ```
   rm unwanted_file.txt
   ```

7. **View File Content (`cat`)**:
   - Command: `cat filename.txt`
   - Explanation: Display the contents of a file. For example:
   ```
   cat my_text_file.txt
   ```

8. **Change File Permissions (`chmod`)**:
   - Command: `chmod permissions file`
   - Explanation: Change the permissions of a file. For example:
   ```
   chmod 644 myfile.txt
   ```

9. **Change File Ownership (`chown`)**:
   - Command: `chown user:group file`
   - Explanation: Change the owner and group of a file. For example:
   ```
   chown username:groupname myfile.txt
   ```

**Text Processing Commands:**

10. **Search for Text in Files (`grep`)**:
    - Command: `grep "search_text" file_to_search.txt`
    - Explanation: Find specific text within a file. For example:
    ```
    grep "important keyword" document.txt
    ```

11. **Display the First Few Lines of a File (`head`)**:
    - Command: `head filename.txt`
    - Explanation: Display the first few lines of a file. For example:
    ```
    head my_text_file.txt
    ```

12. **Display the Last Few Lines of a File (`tail`)**:
    - Command: `tail filename.txt`
    - Explanation: Display the last few lines of a file. For example:
    ```
    tail my_text_file.txt
    ```

13. **Sort and Display Lines of Text Files (`sort`)**:
    - Command: `sort filename.txt`
    - Explanation: Sort and display lines in a text file in alphabetical order. For example:
    ```
    sort names.txt
    ```

**Working with Archives:**

14. **List Contents of a Tarball (`tar`)**:
    - Command: `tar -tvf archive_name.tar`
    - Explanation: View the contents of a tarball without extracting it. For example:
    ```
    tar -tvf my_archive.tar
    ```

**Working Directories:**

15. **Navigate to a Directory (`cd`)**:
    - Command: `cd /path/to/directory`
    - Explanation: Change your current directory to the specified path. For example:
    ```
    cd /home/username/documents
    ```

**Process Management:**

16. **List Running Processes (`ps`)**:
    - Command: `ps`
    - Explanation: List the currently running processes. For example:
    ```
    ps
    ```

17. **Terminate a Process (`kill`)**:
    - Command: `kill process_id`
    - Explanation: Stop or terminate a running process by specifying its process ID. For example:
    ```
    kill 12345
    ```

**Disk Space and Usage:**

18. **Display Disk Space Usage (`df`)**:
    - Command: `df`
    - Explanation: Display the disk space usage on the file system. For example:
    ```
    df
    ```

19. **Display File and Directory Space Usage (`du`)**:
    - Command: `du -h directory_to_check`
    - Explanation: Display the space used by a directory and its subdirectories. For example:
    ```
    du -h /path/to/directory
    ```

**Downloading Files:**

20. **Download a File from the Internet (`wget`)**:
    - Command: `wget URL`
    - Explanation: Download a file from a specified URL. For example:
    ```
    wget https://example.com/file-to-download.txt
    ```
