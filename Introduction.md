## Introduction to Coding Exercise

Welcome to your first coding exercise! In this guide, you'll learn how to set up your development environment by installing Java, Maven, Python, VS Code, and Git Bash. By the end of this exercise, you'll have all the essential tools needed to start coding.

(Note: This guide assumes you are using a Windows environment.)

---

### Introduction to Command Line Interface (CLI) and File System

#### Command Line Interface (CLI)

The Command Line Interface (CLI) is a text-based interface used to interact with your computer. Unlike a graphical user interface (GUI) where you interact with windows, icons, and menus, the CLI requires you to type commands to perform tasks. Here are a few key points about the CLI:

- **Commands:** You enter specific text commands to perform operations like navigating directories, copying files, or running programs.
- **Efficiency:** For many tasks, especially repetitive ones, the CLI can be more efficient than the GUI.
- **Control:** The CLI offers more control over your system and software configurations.

#### File System

The file system is the way an operating system organizes and manages files and directories on your computer. Here are some key concepts:

- **Directories (Folders):** Containers for files and other directories. They help organize your files in a hierarchical structure.
- **Paths:** The address of a file or directory in the file system. It can be absolute (from the root of the file system) or relative (from the current directory).
- **Files:** Units of data storage, which can be text documents, executable programs, images, etc.

---

### Step-by-Step Installation Guide with Explanations

Now, let's elaborate on each step of the installation process and explain what each tool is used for.

---

### Step 1: Install Java

**What is Java?**

Java is a high-level, object-oriented programming language used for building cross-platform applications. It is widely used in enterprise environments and for developing Android applications.

**Installation Steps:**

1. **Download Java Development Kit (JDK):**
   - Go to the [Java SE Downloads page](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html).
   - Choose the appropriate JDK for your operating system and download it.
   - ![Add screenshot]

2. **Install JDK:**
   - Run the downloaded installer and follow the instructions to install Java.
   - **Set up the environment variables:**
     - Open the System Properties (Right-click My Computer/This PC > Properties).
     - ![Add screenshot]
     - Click on Advanced system settings > Environment Variables.
     - ![Add screenshot]
     - Under System variables, click New and add `JAVA_HOME` with the path to your JDK installation (e.g., `C:\Program Files\Java\jdk-11.0.x`).
     - ![Add screenshot]
     - Find the `Path` variable, click Edit, and add `%JAVA_HOME%\bin`.
     - ![Add screenshot]

3. **Verify the Installation:**
   - Open a command prompt (Cmd) and type `java -version`. You should see the installed Java version.
   - ![Add screenshot]

**How to Use Java:**

1. Open VS Code.
2. Create a new file named `HelloWorld.java`.
3. Add the following code:

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

4. Save the file and open a terminal in VS Code.
5. Navigate to the directory containing `HelloWorld.java` using the `cd` command.
6. Compile the program by typing `javac HelloWorld.java`.
   - ![Add screenshot]
7. Run the program by typing `java HelloWorld`. You should see "Hello, World!" printed to the terminal.
   - ![Add screenshot]

---

### Step 2: Install Maven

**What is Maven?**

Maven is a build automation tool primarily used for Java projects. It manages project dependencies, builds the project, and generates reports and documentation.

**Installation Steps:**

1. **Download Maven:**
   - Go to the [Maven Downloads page](https://maven.apache.org/download.cgi).
   - Download the binary zip archive for your operating system.
   - ![Add screenshot]

2. **Install Maven:**
   - Extract the downloaded zip file to a directory (e.g., `C:\Program Files\Maven`).
   - ![Add screenshot]

3. **Set Up Environment Variables:**
   - Open the System Properties (as done in the Java installation step).
   - Click on Advanced system settings > Environment Variables.
   - ![Add screenshot]
   - Under System variables, click New and add `MAVEN_HOME` with the path to your Maven installation (e.g., `C:\Program Files\Maven\apache-maven-3.x.x`).
   - ![Add screenshot]
   - Find the `Path` variable, click Edit, and add `%MAVEN_HOME%\bin`.
   - ![Add screenshot]

4. **Verify the Installation:**
   - Open a command prompt and type `mvn -version`. You should see the installed Maven version.
   - ![Add screenshot]

**How to Use Maven:**

1. Go to the [Spring Initializr](https://start.spring.io/).
2. Fill in the details for your project (e.g., Group, Artifact, Name).
3. Choose the dependencies you need for your project.
4. Click "Generate" to download a zip file of your project.
   - ![Add screenshot]
5. Extract the downloaded zip file to a directory.
6. Open a terminal in that directory.
7. Run `mvn clean install` to build the project.
   - ![Add screenshot]

---

### Step 3: Install Python

**What is Python?**

Python is a high-level, interpreted programming language known for its readability and versatility. It is widely used for web development, data analysis, artificial intelligence, scientific computing, and more.

**Installation Steps:**

1. **Download Python:**
   - Go to the [Python Downloads page](https://www.python.org/downloads/).
   - Choose the latest version for your operating system and download it.
   - ![Add screenshot]

2. **Install Python:**
   - Run the downloaded installer and ensure you check the box to add Python to PATH.
   - Follow the installation instructions.
   - ![Add screenshot]

3. **Verify the Installation:**
   - Open a command prompt and type `python --version` or `python3 --version`. You should see the installed Python version.
   - ![Add screenshot]

**How to Use Python:**

1. Open VS Code.
2. Create a new file named `hello_world.py`.
3. Add the following code:

```python
print("Hello, World!")
```

4. Save the file and open a terminal in VS Code.
5. Navigate to the directory containing `hello_world.py` using the `cd` command.
6. Run the program by typing `python hello_world.py` or `python3 hello_world.py`. You should see "Hello, World!" printed to the terminal.
   - ![Add screenshot]

---

### Step 4: Install Visual Studio Code (VS Code)

**What is Visual Studio Code (VS Code)?**

VS Code is a lightweight but powerful source code editor that supports multiple programming languages and comes with built-in support for JavaScript, TypeScript, and Node.js. It has a rich ecosystem of extensions for other languages, debugging, and version control.

**Installation Steps:**

1. **Download VS Code:**
   - Go to the [VS Code Downloads page](https://code.visualstudio.com/Download).
   - Choose the version for your operating system and download it.
   - ![Add screenshot]

2. **Install VS Code:**
   - Run the downloaded installer and follow the instructions to install VS Code.
   - ![Add screenshot]

3. **Launch VS Code:**
   - Open VS Code and customize the settings as needed.
   - ![Add screenshot]

**How to Use VS Code:**

1. Open VS Code.
2. Use the Explorer on the left to navigate your files.
3. Use the terminal integrated in VS Code to run commands.
4. Install extensions to add support for more programming languages and tools.
   - ![Add screenshot]

---

### Step 5: Install Git Bash

**What is Git Bash?**

Git Bash provides a Unix-style command-line interface for Windows users, along with Git, which is a version control system that lets you track changes to your code and collaborate with others.

**Installation Steps:**

1. **Download Git:**
   - Go to the [Git Downloads page](https://git-scm.com/downloads).
   - Choose the version for your operating system and download it.
   - ![Add screenshot]

2. **Install Git Bash:**
   - Run the downloaded installer and select Git Bash during the installation process.
   - ![Add screenshot]

3. **Verify the Installation:**
   - Open Git Bash and type `git --version`. You should see the installed Git version.
   - ![Add screenshot]

**How to Use Git Bash:**

1. Open Git Bash.
2. Use `git init` to initialize a new Git repository.
3. Use `git clone [repository URL]` to clone an existing repository.
4. Use `git add`, `git commit`, and `git push` to manage your code changes.
   - ![Add screenshot]

---

### Creating a "Hello, World!" Program

To verify that everything is set up correctly, let's create a simple "Hello, World!" program in Java and Python.

#### Java

1. Open VS Code.
2

. Create a new file named `HelloWorld.java`.
3. Add the following code:

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

4. Save the file and open a terminal in VS Code.
5. Navigate to the directory containing `HelloWorld.java` using the `cd` command.
6. Compile the program by typing `javac HelloWorld.java`.
   - ![Add screenshot]
7. Run the program by typing `java HelloWorld`. You should see "Hello, World!" printed to the terminal.
   - ![Add screenshot]

#### Python

1. Open VS Code.
2. Create a new file named `hello_world.py`.
3. Add the following code:

```python
print("Hello, World!")
```

4. Save the file and open a terminal in VS Code.
5. Navigate to the directory containing `hello_world.py` using the `cd` command.
6. Run the program by typing `python hello_world.py` or `python3 hello_world.py`. You should see "Hello, World!" printed to the terminal.
   - ![Add screenshot]

---

### Conclusion

Congratulations! You've successfully set up your development environment with Java, Maven, Python, VS Code, and Git Bash. Each of these tools plays a crucial role in modern software development, and now you are ready to start your coding journey. Happy coding!
```
