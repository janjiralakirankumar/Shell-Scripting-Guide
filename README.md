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
## Introduction to VI

**Introduction to Vi:**

Vi (pronounced "vee-eye") is a text editor that is commonly found on Unix and Linux systems. It's a versatile and powerful text editor that operates in a terminal or command-line environment. Vi is known for its efficiency, especially when working with configuration files, scripts, and code.

Vi is a modal editor, which means it has different modes for different tasks. There are primarily three modes in Vi:

1. **Command Mode:** This is the default mode when you open a file with Vi. In this mode, you can navigate the document, issue commands, and manipulate text.

2. **Insert Mode:** In Insert Mode, you can actually type and edit text. You enter Insert Mode by pressing "i" or other keys like "a," "I," "o," or "O" depending on where you want to insert text.

3. **Visual Mode:** Visual Mode is used for selecting and manipulating text. It's helpful when you want to copy, cut, or replace text.

Here's how you typically use Vi:

- Open a file with `vi filename`.
- Start in Command Mode.
- Switch to Insert Mode to edit text.
- Return to Command Mode to save, exit, or issue commands.

Vi has a learning curve, but once you become proficient, it's a highly efficient text editor.

**Basic Vi Commands:**

1. **Opening a File with Vi:**
   To open a file with Vi, use the command:
   ```
   vi filename
   ```
   For example, to open a file named "document.txt":
   ```
   vi document.txt
   ```

2. **Switch to Insert Mode:**
   To start typing or editing text, switch to Insert Mode by pressing "i." You can use other keys like "a," "I," "o," or "O" for different insertion points.

3. **Save Changes in Command Mode:**
   - To save changes, return to Command Mode (if not already there) by pressing "Esc" and then type `:w` and press Enter.
   - Example:
     ```
     :w
     ```

4. **Save and Quit:**
   To save changes and exit Vi, return to Command Mode and type `:wq` and press Enter.
   - Example:
     ```
     :wq
     ```

5. **Quit Without Saving:**
   If you want to exit Vi without saving changes, return to Command Mode and type `:q!` and press Enter.
   - Example:
     ```
     :q!
     ```

6. **Navigation in Command Mode:**
   - Move the cursor with arrow keys or use "h," "j," "k," and "l" for left, down, up, and right, respectively.
   - Jump to the beginning of a line with `0`.
   - Jump to the end of a line with `$`.

7. **Delete Text:**
   - Delete the character under the cursor with `x`.
   - Delete a line with `dd`.

8. **Copy and Paste in Command Mode:**
   - Copy (yank) a line with `yy`.
   - Paste (put) a line with `p`.

9. **Undo and Redo:**
   - Undo with `u`.
   - Redo with `Ctrl-r`.

10. **Search in Command Mode:**
    - Search for text with `/search_term`. Use `n` to find the next occurrence and `N` to find the previous one.

11. **Replace Text:**
    - Replace the character under the cursor with `r`.
    - Replace text with `c` followed by a motion command. For example, `cw` changes the word under the cursor.

12. **Visual Mode:**
    - Enter Visual Mode by pressing `v`. This allows you to select text for copying or other operations.


## File Permissions with example:

File permissions in Unix-like operating systems are represented by a set of three categories (user, group, others) and three permission types (read, write, execute). These permissions determine who can access and perform actions on a file.

Here's how it works, along with an example and calculation:

1. **Permission Types:**

   - **Read (r)**: Allows viewing or reading the contents of a file.
   - **Write (w)**: Allows modifying the file or creating new files in a directory.
   - **Execute (x)**: Allows running a script or traversing (entering) a directory.

2. **Permission Categories:**

   - **User (Owner)**: Represents the file's owner.
   - **Group**: Refers to a specific group of users who share the same permissions.
   - **Others (World)**: Encompasses everyone else.

**Example:**
Let's consider a file named "example.txt" with the following permissions: `rw-r--r--`. This means:

- The **owner** (user) has read (r) and write (w) permissions.
- The **group** has read (r) permission.
- **Others** (everyone else) have read (r) permission.

**Numeric Representation Calculation:**

You can represent these permissions numerically by calculating the sum of permission values:

- Read (r) is represented as 4.
- Write (w) is represented as 2.
- Execute (x) is represented as 1.

For the owner, the calculation is: `r (4) + w (2) = 6`. So, the owner has a numeric representation of 6.

For the group and others, they only have read permission, so their numeric representation is: `r (4)`.

Therefore, the numeric representation of the file's permissions is: `644`. This is commonly referred to as the "octal" representation.

So, "example.txt" has permissions of `rw-r--r--` (symbolic) or `644` (numeric). The owner can read and write, but the group and others can only read the file.

## Writing the first shell script by setting permissions and executing it.

To write a shell script, you can create a text file with the extension `.sh` and then use a text editor to enter your script. After writing the script, you need to set the appropriate permissions to make it executable, and then you can run it. Here's a step-by-step guide with an example:

**Step 1: Write a Shell Script**

1. Open a text editor (such as Vi, Nano, or Gedit) and create a new file with a `.sh` extension. For example, you can create a file named `myscript.sh`:
   
   ```bash
   touch myscript.sh
   ```

2. Use the text editor to write your shell script. Here's a simple example of a shell script that prints "Hello, World!" to the terminal:

   ```bash
   #!/bin/bash
   echo "Hello, World!"
   ```

   Save the file when you're done.

**Step 2: Set Permissions**

Before you can execute a shell script, you need to make it executable. To do this, you can use the `chmod` command to add the execute permission to the script file.

1. Open a terminal and navigate to the directory where your script is located. For example, if your script is in your home directory, you can use the `cd` command:

   ```bash
   cd ~
   ```

2. Use the `chmod` command to add execute permission to your script:

   ```bash
   chmod +x myscript.sh
   ```

**Step 3: Execute the Shell Script**

Now that your script is executable, you can run it from the terminal.

1. In the terminal, navigate to the directory where your script is located, if you're not already there.

2. To run the script, simply type its name and press Enter:

   ```bash
   ./myscript.sh
   ```

   The `./` prefix is used to indicate that you want to run a script from the current directory.

3. You should see the output of your script in the terminal:

   ```bash
   Hello, World!
   ```

That's it! You've successfully written a shell script, set its permissions, and executed it.

Remember that you can write more complex shell scripts to automate tasks, perform system administration, or any other custom tasks you need. The key is to write the shell commands in the script file, set the execution permission, and run the script when needed.

## Variables in Shell scripting:

In shell scripting, variables are used to store and manipulate data. They are fundamental components for creating dynamic and reusable scripts. Shell scripting supports both **global** and **local** variables, and they can hold various types of data, including text and numbers.

Here are the basics of working with variables in shell scripting:

**1. Variable Naming Conventions:**
   - Variable names are case-sensitive and consist of letters, numbers, and underscores (A-Z, a-z, 0-9, and _).
   - A variable name cannot start with a number.
   - It's a good practice to use descriptive and meaningful names for variables.

**2. Variable Assignment:**
   - You can assign a value to a variable using the `=` operator, without spaces on either side of the `=`. For example:
     ```bash
     my_variable="Hello, World!"
     ```

**3. Accessing Variable Values:**
   - To access the value of a variable, you prepend a `$` symbol to its name. For example:
     ```bash
     echo $my_variable
     ```

**4. Quoting Variable Values:**
   - It's a good practice to enclose variable names in double quotes to handle spaces and special characters properly. For example:
     ```bash
     echo "$my_variable"
     ```

**5. Special Variables:**
   - Shell scripts have access to various special variables such as `$0` (script name), `$1`, `$2`, ... (command line arguments), and `$#` (number of arguments).

**6. Readonly Variables:**
   - You can mark a variable as readonly using the `readonly` command to prevent its value from being changed later in the script. For example:
     ```bash
     readonly my_const="This is a constant value."
     ```

**7. Unsetting Variables:**
   - To remove the value of a variable, use the `unset` command. For example:
     ```bash
     unset my_variable
     ```

**8. Variable Types:**
   - By default, shell scripting uses string variables, but you can perform arithmetic operations using `$(( ))` for integer variables.

**9. Global vs. Local Variables:**
   - In shell scripting, variables are global by default. However, you can limit a variable's scope to a specific function or block by declaring it as `local` within that function.

Here's a simple example of using variables in a Bash script:

```bash
#!/bin/bash

# Variable assignment
my_name="John"
my_age=30

# Accessing and displaying variables
echo "My name is $my_name and I am $my_age years old."

# Special variables
echo "Script name: $0"
echo "First argument: $1"
echo "Number of arguments: $#"
```

In this script, we assign values to two variables, `my_name` and `my_age`. We then access and display their values. The special variables `$0`, `$1`, and `$#` provide information about the script and its command line arguments.

Variables are essential for making shell scripts dynamic and flexible. You can use them to store user input, configuration settings, and intermediate results, among other things.

## Arithmetical Calculations:

**Basic Arithmetic:**

You can do simple math like addition, subtraction, multiplication, division, and finding the remainder using `+`, `-`, `*`, `/`, and `%` operators, respectively. For example:

```bash
result=$((5 + 3))
echo "5 + 3 equals $result"
```

**Increment and Decrement:**

You can increase or decrease a number using `++` and `--`. For instance:

```bash
num=5
((num++))  # This increases num by 1
((num--))  # This decreases num by 1
echo "After increment and decrement, num is now $num"
```

**Math Expressions:**

You can use parentheses for more complicated math expressions:

```bash
total=$((2 * (3 + 4)))
echo "2 times (3 plus 4) is $total"
```

**Comparison and Logical Operators:**

You can use comparison operators (`>`, `<`, `>=`, `<=`, `==`, `!=`) and logical operators (`&&` for AND, `||` for OR) to make decisions in your scripts:

```bash
a=5
b=7
((is_greater = a > b))
echo "Is 'a' greater than 'b'? $is_greater"
```

```bash
x=10
y=5
((is_true = (x > y) && (x % 2 == 0)))
echo "Is 'x' greater than 'y' and even? $is_true"
```

**Using Variables:**

You can perform math with variables and store the result in another variable:

```bash
num1=8
num2=3
((sum = num1 + num2))
echo "The sum of num1 and num2 is $sum"
```

These simple examples show how you can use basic arithmetic, increment or decrement values, perform more complex math, make comparisons, and work with variables in shell scripts.

## Write a shell script to determine the largest number among three integer numbers

```bash
#!/bin/bash

# Input three integers from the user
echo "Enter three integers:"
read num1
read num2
read num3

# Check which number is the largest
if [ "$num1" -gt "$num2" ] && [ "$num1" -gt "$num3" ]; then
  largest="$num1"
elif [ "$num2" -gt "$num1" ] && [ "$num2" -gt "$num3" ]; then
  largest="$num2"
else
  largest="$num3"
fi

# Display the result
echo "The largest number among $num1, $num2, and $num3 is $largest."
```

You can save this script in a file, for example, "find_largest.sh," make it executable with the `chmod +x find_largest.sh` command, and then run it. Here's how you can run the script:

```bash
$ ./find_largest.sh
```

The script will prompt you to enter three integers, and it will then determine and display the largest number among the three. For example:

```
Enter three integers:
15
8
23
The largest number among 15, 8, and 23 is 23.
```
