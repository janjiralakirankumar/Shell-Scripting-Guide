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

**4. Global vs. Local Variables:**
   - In shell scripting, variables are global by default. However, you can limit a variable's scope to a specific function or block by declaring it as `local` within that function.

Here's a simple example of using variables in a Bash script:

```bash
#!/bin/bash

# Variable assignment
my_name="John"
my_age=30

# Accessing and displaying variables
echo "My name is $my_name and I am $my_age years old."
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
