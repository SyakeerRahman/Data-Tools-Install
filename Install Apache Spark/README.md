Prerequisites

A system running Windows 10
A user account with administrator privileges (required to install software, modify file permissions, and modify system PATH)
Command Prompt or Powershell
A tool to extract .tar files, such as 7-Zip
Install Apache Spark on Windows
Installing Apache Spark on Windows 10 may seem complicated to novice users, but this simple tutorial will have you up and running. If you already have Java 8 and Python 3 installed, you can skip the first two steps.

## Step 1: Install Java 8

Apache Spark requires Java 8. You can check to see if Java is installed using the command prompt.

Open the command line by clicking Start > type cmd > click Command Prompt.

Type the following command in the command prompt:

java -version

If Java is installed, it will respond with the following output:
![image](https://github.com/SyakeerRahman/Data-Tools-Install/assets/105381652/51817cc8-04d9-41f4-b77d-e006eca922c3)

Your version may be different. The second digit is the Java version – in this case, Java 8.

If you don’t have Java installed:

1. Open a browser window, and navigate to https://java.com/en/download/.

2. Click the Java Download button and save the file to a location of your choice.

3. Once the download finishes double-click the file to install Java.

## Step 2: Install Python

1. To install the Python package manager, navigate to https://www.python.org/ in your web browser.

2. Mouse over the Download menu option and click Python 3.8.3. 3.8.3 is the latest version at the time of writing the article.

3. Once the download finishes, run the file.

4. Near the bottom of the first setup dialog box, check off Add Python 3.8 to PATH. Leave the other box checked.

5. Next, click Customize installation.

   ![image](https://github.com/SyakeerRahman/Data-Tools-Install/assets/105381652/a5c374d6-ff99-4715-8abb-d78aca896d5e)

6. You can leave all boxes checked at this step, or you can uncheck the options you do not want.

7. Click Next.

8. Select the box Install for all users and leave other boxes as they are.

9. Under Customize install location, click Browse and navigate to the C drive. Add a new folder and name it Python.

10. Select that folder and click OK.

11. Click Install, and let the installation complete.

12. When the installation completes, click the Disable path length limit option at the bottom and then click Close.

13. If you have a command prompt open, restart it. Verify the installation by checking the version of Python:

python --version

The output should print Python 3.8.3.

