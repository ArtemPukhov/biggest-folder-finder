<!DOCTYPE html>
<html>
<head>
 
</head>
<body>
  <h1>Description</h1>
  <p>The Java program calculates the total size of a folder and its subfolders by utilizing the Fork/Join framework. The program performs the following steps:</p>
  <ul>
    <li>Parses the command-line arguments to retrieve the folder path and size limit.</li>
    <li>Creates a File object representing the specified folder.</li>
    <li>Creates a Node object with the folder and size limit.</li>
    <li>Measures the start time of the calculation.</li>
    <li>Creates a FolderSizeCalculator object with the root node.</li>
    <li>Creates a ForkJoinPool to manage the parallel computation.</li>
    <li>Invokes the FolderSizeCalculator to calculate the folder size.</li>
    <li>Prints the root node, which contains the total size of the folder and its subfolders.</li>
    <li>Calculates the duration of the program execution and prints it in milliseconds.</li>
  </ul>

  <h2>Requirements</h2>
  <p>To run the program, ensure that you have the following:</p>
  <ul>
    <li>Java Development Kit (JDK) installed on your system.</li>
  </ul>

  <h2>Usage</h2>
  <p>The program can be executed either by using the command line or by running the compiled JAR file. It requires two parameters: -l (limit) and -d (folder path).</p>

  <h3>Using Command Line</h3>
  <ol>
    <li>Open a command prompt or terminal.</li>
    <li>Navigate to the directory containing the compiled JAR file.</li>
    <li>Execute the following command:</li>
  </ol>
  <code>java -jar program.jar -l &lt;sizeLimit&gt; -d &lt;folderPath&gt;</code>
  <p>Replace &lt;sizeLimit&gt; with the maximum size limit for each node (with Multipliers {'B', 'K', 'M', 'G', 'T'}) and &lt;folderPath&gt; with the path to the folder you want to calculate the size for.</p>
  <p>Example:</p>
  <code>java -jar program.jar -l 10M -d /path/to/folder</code>
  <p>The program will start executing and display the total size of the folder and its subfolders.</p>
  <p>After the program finishes, it will display the duration of the execution in milliseconds.</p>

  <h3>Using Compiled JAR File</h3>
  <ol>
    <li>Ensure that you have the compiled JAR file (program.jar) in the desired location.</li>
    <li>Open a command prompt or terminal.</li>
    <li>Navigate to the directory containing the JAR file.</li>
    <li>Execute the following command:</li>
  </ol>
  <code>java -jar program.jar -l &lt;sizeLimit&gt; -d &lt;folderPath&gt;</code>
  <p>Replace &lt;sizeLimit&gt; with the maximum size limit for each node (with Multipliers {'B', 'K', 'M', 'G', 'T'}) and &lt;folderPath&gt; with the path to the folder you want to calculate the size for.</p>
  <p>Example:</p>
  <code>java -jar program.jar -l 10M -d /path/to/folder</code>
  <p>The program will start executing and display the total size of the folder and its subfolders.</p>

  <p>After the program finishes, it will display the duration of the execution in milliseconds.</p>
  <h2>Customization</h2>
  <p>If you want to customize the program, you can modify the following parameters:</p>
  <ul>
    <li><code>-l &lt;sizeLimit&gt;</code>: Set the maximum size limit for each node (with Multipliers {'B', 'K', 'M', 'G', 'T'}).</li>
    <li><code>-d &lt;folderPath&gt;</code>: Set the path to the folder you want to calculate the size for.</li>
  </ul>
  <p>Note: The program assumes that the specified folder exists and is accessible. Ensure that you have the necessary permissions to access the folder and its contents.</p>
  <h2>Troubleshooting</h2>
  <ul>
    <li>If the program encounters any errors or exceptions, it will display error messages or stack traces. Check if the folder path is valid and accessible, and ensure that you provide valid command-line arguments.</li>
    <li>If the program takes a long time to execute or hangs, check if the specified folder contains a large number of files or subfolders, as it may require more time for computation.</li>
  </ul>
  <h2>License</h2>
  <p>This program is released under the MIT License. Feel free to modify and distribute it according to your needs.</p>
</body>
</html>
