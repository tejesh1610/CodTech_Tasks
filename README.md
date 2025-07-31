# File Handling Utility

This Java-based utility offers a simple and modular approach to handling text files, supporting reading, writing, and modification operations with robust error management. Designed for ease of integration into larger projects, it demonstrates effective use of Java's core file I/O capabilities.

## Features

- Read content from `.txt` files line by line
- Append new data to an existing file
- Overwrite a file's entire contents
- Work with both relative and absolute file paths
- Handle I/O exceptions with clarity and control

## Technologies Used

- Java 8 or higher
- Core Java file I/O (`BufferedReader`, `FileWriter`, `File`)
- Object-oriented design principles

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/tejesh1610/File-Handing-Utility.git

2. Navigate to the Project Folder
Bash
cd File-Handing-Utility

3. Compile and Run
Use any Java-compatible IDE or compile manually using:
Bash
javac FileHandler.java
java FileHandler


Example Usage
FileHandler handler = new FileHandler("example.txt");
handler.write("This is a new line");
String content = handler.read();
System.out.println(content);

License
This project is distributed under the MIT License. Please refer to the LICENSE file for more details.
Contributions
Contributions and feedback are welcome. You can open an issue for bugs or suggestions, or submit a pull request with improvements or new features.

created by Tejesh - with a focus on clean design ,practical utility, and extensibility.
