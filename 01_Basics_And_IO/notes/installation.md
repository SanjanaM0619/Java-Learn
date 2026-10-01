## Steps to instal Java
## Prerequisites

- [Visual Studio Code](https://code.visualstudio.com/)
- [Java JDK 17+](https://www.oracle.com/java/technologies/downloads/#java17) (Oracle JDK)

## Installation Steps

### 1. Install Oracle JDK

1. Go to [Oracle's Java Download page](https://www.oracle.com/java/technologies/downloads/#java17).
2. Select your OS (Windows / macOS / Linux) and download the **JDK** (not just JRE).
3. **Accept the License Agreement** and download the installer.
4. Run the installer and follow the prompts.
   - **Windows:** Default path is `C:\Program Files\Java\jdk-17` (or `jdk-21`).
   - **macOS:** Drag the JDK into `/Library/Java/JavaVirtualMachines/`.
   - **Linux:** Extract to `/opt/java/` or `/usr/lib/jvm/` and set `JAVA_HOME`.
5. Verify the installation by opening a terminal:

   ```bash
   java -version  
   You should see output like java version "17.0.x" 2024-xx-xx LTS   
   
### Install the extension pack for java
1. Open VS Code.
2. Go to the Extensions view (Ctrl+Shift+X / Cmd+Shift+X).
3. Search for Extension Pack for Java by Microsoft.
4. Click Install.

### Configure JDK Path 
1. Open Settings (Ctrl+, / Cmd+,).
2. Search for java.jdt.ls.java.home.
3. Set the value to your Oracle JDK path, e.g.:
4. Windows: C:\Program Files\Java\jdk-17
5. macOS: /Library/Java/JavaVirtualMachines/jdk-17.jdk/Contents/Home
6. Linux: /opt/java/jdk-17 (or wherever you extracted it)

### Create a new Project
1. Open a folder in VS Code.
2. Open the Command Palette (Ctrl+Shift+P / Cmd+Shift+P).
3. Type Java: Create Java Project.
4. Choose Create a Standalone Java File or Maven/Gradle project.
5. Name your project and select a location.

# Hello World Program
In Java the class name and the class must match the file name 
**Reason**:Java uses the class name to find and run code.
If the names do not match , Java will give an error and the program will not run.
```java
public class Main{
    public static void main(string[] args){
        System.out.println("Hello World");
    }
}
```
Output is : Hello World