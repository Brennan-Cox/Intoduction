## Introduction to Coding Exercise

Welcome to your first coding exercise! In this guide, you'll learn how to set up your development environment by installing Java, Maven, Python, VS Code, and Git Bash. By the end of this exercise, you'll have all the essential tools needed to start coding.

(Note: This guide assumes you are using a Windows environment.)
(Note: Ask chat gpt if you have any questions about any of these steps [chatgpt.com](https://chat.openai.com/chat))

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
   - Choose the latest jdk and Windows, then choose either the .exe or .msi installer
   - ![image](https://github.com/Brennan-Cox/Intoduction/assets/95318091/a2fcae1b-2382-45aa-b843-861ec5fc5b3a)

2. **Install JDK:**
   - Run the downloaded installer and follow the instructions to install Java. (Just accecpt all defaults)

3. **Verify the Installation:**
   - Open a command prompt (Cmd) and type `java -version`. You should see the installed Java version.
   - ![image](https://github.com/Brennan-Cox/Intoduction/assets/95318091/07bd3cbd-5872-4c73-867f-048587adc639)

**How to Use Java:**

1. Open VS Code. (A later step)
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
7. Run the program by typing `java HelloWorld`. You should see "Hello, World!" printed to the terminal.
8. Or compile and run the program in one step, using `java HelloWorld.java`

---

### Step 2: Install Maven

**What is Maven?**

Maven is a build automation tool primarily used for Java projects. It manages project dependencies, builds the project, and generates reports and documentation. (Makes things much less work)

**Installation Steps:**

1. **Download Maven:**
   - Go to the [Maven Downloads page](https://maven.apache.org/download.cgi).
   - Download the binary zip archive.

2. **Install Maven:**
   - Extract the downloaded zip file to a directory (e.g., `C:\Program Files\Maven`).
   - ![image](https://github.com/Brennan-Cox/Intoduction/assets/95318091/7c21b42f-1363-459c-a492-0bb138c43f57)
     
3. **Set Up Environment Variables:**
   - Open the System Properties (windows button + env + enter)
   - Click on Advanced system settings > Environment Variables.
   - ![image](https://github.com/Brennan-Cox/Intoduction/assets/95318091/f457a0f2-8f8e-4214-9915-6ba331ae3576)
   - Find the `Path` variable, click Edit, and add `%MAVEN_HOME%\bin`.
   - ![image](https://github.com/Brennan-Cox/Intoduction/assets/95318091/d1444792-403e-43f2-bcb3-6286b538ec31)

4. **Verify the Installation:**
   - Open a command prompt and type `mvn -version`. You should see the installed Maven version.
   - ![image](https://github.com/Brennan-Cox/Intoduction/assets/95318091/97a8c7b5-5ec2-41e7-8f9a-b2ab9c30f9a5)
     
**How to Use Maven:**

1. Go to the [Spring Initializr](https://start.spring.io/).
2. Fill in the details for your project (e.g., Group, Artifact, Name).
3. Choose the dependencies you need for your project.
4. Click "Generate" to download a zip file of your project.
   - ![image](https://github.com/Brennan-Cox/Intoduction/assets/95318091/7cc8942f-ea5d-4849-a6a8-8d9268c27e0c)
5. Extract the downloaded zip file to a directory.
   - ![image](https://github.com/Brennan-Cox/Intoduction/assets/95318091/fdf55739-3b99-4f8f-8a82-b38ceb6373f2)
7. Open a terminal in that directory.
   - Right click a-cool-project
   - Left click open in terminal
9. Run `mvn clean install` to build the project.
   - ![image](https://github.com/Brennan-Cox/Intoduction/assets/95318091/f5758ea8-3224-4272-ba2b-741857d8d367)
   - If this was a real project with tests then those would have run, we will use mvn wayyyyy later in the demos. (don't worry about it for now)

---

### Step 3: Install Python

**What is Python?**

Python is a high-level, interpreted programming language known for its readability and versatility. It is widely used for web development, data analysis, artificial intelligence, scientific computing, and more. (It is a simpler designed language and is what we will do a lot with)

**Installation Steps:**

1. **Download Python:**
   - Go to the [Python Downloads page](https://www.python.org/downloads/).
   - Choose the latest version for your operating system and download it.
   - ![image](https://github.com/Brennan-Cox/Intoduction/assets/95318091/882a19f3-de01-4342-b64a-f097dd1b054c)
   - 
   - If installation successful and asked to disable path limit close for now. (this is like an address limit to how long your street address can be)

2. **Install Python:**
   - Run the downloaded installer and ensure you check the box to add Python to PATH.
   - Follow the installation instructions.
   - ![image](https://github.com/Brennan-Cox/Intoduction/assets/95318091/15090f08-96c7-4741-b9d7-28b01f118a7b)

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
