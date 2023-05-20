Description
The Java program calculates the total size of a folder and its subfolders by utilizing the Fork/Join framework. The program performs the following steps:

Parses the command-line arguments to retrieve the folder path and size limit.
Creates a File object representing the specified folder.
Creates a Node object with the folder and size limit.
Measures the start time of the calculation.
Creates a FolderSizeCalculator object with the root node.
Creates a ForkJoinPool to manage the parallel computation.
Invokes the FolderSizeCalculator to calculate the folder size.
Prints the root node, which contains the total size of the folder and its subfolders.
Calculates the duration of the program execution and prints it in milliseconds.
Requirements
To run the program, ensure that you have the following:

Java Development Kit (JDK) installed on your system.

Usage
The program can be executed either by using the command line or by running the compiled JAR file. It requires two parameters: -l (limit) and -d (folder path).

Using Command Line
Open a command prompt or terminal.

Navigate to the directory containing the compiled JAR file.

Execute the following command:

php
Copy code
java -jar program.jar -l <sizeLimit> -d <folderPath>
Replace <sizeLimit> with the maximum size limit for each node (in bytes) and <folderPath> with the path to the folder you want to calculate the size for.

Example:

bash
Copy code
java -jar program.jar -l 100000000 -d /path/to/folder
The program will start executing and display the total size of the folder and its subfolders.

After the program finishes, it will display the duration of the execution in milliseconds.

Using Compiled JAR File
Ensure that you have the compiled JAR file (program.jar) in the desired location.

Open a command prompt or terminal.

Navigate to the directory containing the JAR file.

Execute the following command:

java -jar program.jar -l <sizeLimit> -d <folderPath>
Replace <sizeLimit> with the maximum size limit for each node (with use Multipliers 'B', 'K', 'M', 'G', 'T') and <folderPath> with the path to the folder you want to calculate the size for.

Example:
  
java -jar program.jar -l 10M -d "/path/to/folder"
The program will start executing and display the total size of the folder and its subfolders.

After the program finishes, it will display the duration of the execution in milliseconds.

Customization
If you want to customize the program, you can modify the following parameters:

-l <sizeLimit>: Set the maximum size limit for each node (with use Multipliers 'B', 'K', 'M', 'G', 'T').
-d <folderPath>: Set the path to the folder you want to calculate the size for.
Note: The program assumes that the specified folder exists and is accessible. Ensure that you have the necessary permissions to access the folder and its contents.

Troubleshooting
If the program encounters any errors or exceptions, it will display error messages or stack traces. Check if the folder path is valid and accessible, and ensure that you provide valid command-line arguments.
If the program takes a long time to execute or hangs, check if the specified folder contains a large number of files or subfolders, as it may require more time for computation.
License
This program is released under the MIT License. Feel free to modify and distribute it according to your needs.
