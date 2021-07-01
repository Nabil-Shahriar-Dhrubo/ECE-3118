Documentation on Git Commands

Submitted By:
Nabil Shahriar Dhrubo

# **1. Git Configuration:**

The Git config command is the first and necessary command used on the Git command line. This command sets the author name and email address to be used with your commits. Git config is also used in other scenarios. 

**Syntax**
```
git config --global user.name "Nusrat-Jahan-ECE"  
git config --global user.email "1710011@student.ruet.ac.bd"
````
# **2. To Check Git Version:**

We can check your current version of Git by running the following command in Git Bash, terminal (Linux, macOS) or command prompt (Windows).

**Syntax:**
```
git --version
````
# **3. Git Initialization**

To create a blank repository, open command line on your desired directory and run the init command as follows:
```
git init
````
# **4. Git Status Command**

The status command is used to display the state of the working directory and the staging area. It also lists the files that you've changed and those you still need to add or commit.

**Syntax:**
```
git status
````
# **5. Git Add Command**

This command is used to add one or more files to staging (Index) area.

**Syntax:**

**i. To add one file:**
```
git add <Filename>  
````
**ii. To add more than one file:**
```
git add*
````
**iii. To add all files:**
```
git add -A
````