# Project 1 - Getting Started with Java and Github: Creating a Menu App
In this project, you will download software that allows you to run Git and submit a simple Java program to demonstrate that you have a development environment. The final step asks you to write a menu application to demonstrate that you can understand user input, Java mathematical statements, and control flow.

## Step 1 - Create a Github account
Go to the [Github website](https://github.com) and create an account. They have [student packs](https://education.github.com/pack) that give you access to many things that would otherwise be very expensive, so I recommend you sign up using your american.edu email address. You can associate a Github account with multiple email addresses.

## Step 2 - Get git
1. Visit the Git [website](https://git-scm.com/downloads) and download the latest Git release for your operating system.
1. Install it, using default settings.
1. As a reference for how to use git, I suggest [Coding Domain](http://codingdomain.com/git/), as it avoids some of the more complicated theory behind git and focuses on the bare minimum practicalities. There are also many good videos, but we will go over some of the basics in class.

**Deliverable 1:** Modify this .md file so that your name and newly obtained Github profile name replaces the text in the lines below.

My Name is: *REPLACE_THIS*

My Github ID is: *REPLACE_THIS*

## Step 2.5 - Become familiar with the command line application for your OS

Each Operating System (OS) has at least one primary application for navigating the system through the command line. These are powerful applications, and allow you to install programs and software libraries or run the programs that you will develop in this course. Every developer should have at least a rudimentary knowledge of how to use the command line application on your system. There are fairly decent introductory videos for how to use the command line options. Many of the commands for both systems are the same (e.g., `cd`, `ls`, `javac`) but there will be some differences in presentation and overall capability.

- On MacOS, this application is called Terminal.
- On Windows, this application is called Powershell.

## Step 3 - Download and install JDK SE 11
1. Go to the <a href="https://www.oracle.com/java/technologies/javase-jdk11-downloads.html">Oracle site</a> and download the JDK SE installer for your OS. 
1. Install it. If you are given the option to install an Integrated Development Environment (IDE) with it, do not install the IDE. Just get the JDK SE.
1. Here's the tricky part. You need to make Java visible to your command line tool. This is called "adding to path," and affects which commands you can run. Think about it this way - it would be pretty annoying if every time you wanted to open a Word document, you had to move that document into the same folder as Word. There is some chance that the installer did this for you, depending on your setup, but likely not. You can verify if Java is available by opening your command line tool (Terminal on Mac or Powershell on PC) and typing `javac` from anywhere (yes, with a 'c' on the end). If the command is recognized, you are in good shape. If not, then you need to add it to the path.
1. This process is different depending on your operating system. Directions for both types of systems can be found at <a href='https://www.java.com/en/download/help/path.xml'>this link</a>.

**Deliverable 2:** In this directory, save a screenshot image showing what happens when you type `java` into your terminal/command line.

## Step 4 - Download and install a development tool
As we discussed in class, you should download and install a powerful IDE or text editor. An IDE will make it easier to perform many coding tasks, but they are more complex applications and it will be more challenging to become familiar with all of the features. There is also a risk that developing all your code in an IDE may make it more challenging to learn the details of writing code on your own - many automated processes that will not always be available exams or technical interviews.

#### IDE

I recommend using an IDE for this course, specifically IntelliJ IDEA. Other IDEs are fine if you are already familiar with them, but all examples in lectures will be using IntelliJ IDEA.

*Pros:* Simplifies development by automating common tasks, highlighting potential errors before you try to build, and has features for building and debugging.

*Cons:* Big, complicated application with many features that we will not use in this class. Hides certain features of the development process that make it difficult to understand what is going on. Will not be available during quizzes, exams, or professional coding interviews in the hiring process.

Examples:

1. IntelliJ IDEA https://www.jetbrains.com/idea/
1. Atom https://ide.atom.io/
1. Eclipse https://www.eclipse.org/downloads/packages/installer
1. Netbeans https://netbeans.org

#### Text Editor

*Pros:* Simple to set up and use, typically extensible, can use the same environment to develop scripts, applications, websites, academic papers, etc. Even if you decide to use an IDE, it's still a good idea to have a powerful text editor available.

*Cons:* Very little is automated unless you extend the capabilities of the system through installed add-ons (e.g., building code, linters). 

I suggest either one of the following:

1. Sublime Text 3 (recommended) https://www.sublimetext.com/
1. Notepad++ https://notepad-plus-plus.org/
1. Visual Studio Code https://code.visualstudio.com/


#### jGRASP (a middle ground)

If you want the simplicity of a good text editor but want to have some of the benefits pre-installed, than there are some good options out there while you are still learning Java. Of these I recommend [jGRASP](https://spider.eng.auburn.edu/user-cgi/grasp/grasp.pl?;dl=download_jgrasp.html) most highly. It can be more challenging to work with larger projects in jGRASP, but it may be less intimidating than IntelliJ.

**Deliverable 3:** In this directory, save a screenshot image showing your installed IDE or text editor open. Then modify the statement below:

My chosen development tool is: *REPLACE_THIS*

## Step 5 - Clone your Repo locally

Because you can see these instructions, that means that you have already followed the link and accepted the assignment. Github classroom has automatically created a repository for you on Github and imported the starting code into it. A full tutorial for how to do this with GitHub is available [here](https://riptutorial.com/github/example/23708/clone-a-repository), but the basic steps are the following:

1. On this page, there is a big button labeled **Code**. If you click it, you get the web URL for this online repo. Copy it. 
1. Open your command line. Navigate to the directory that you want to clone your repo (somewhere on your PC that you keep your projects for this course).
1. Type: `git clone copied_url_from_step_1` and hit enter.
1. Open the directory in Sublime so that you can see the code for this assignment.

## Step 5.5 - Modify the Starter Code

1. You should see a simple - but definitely broken - Java program in the HelloWorld.java file.
1. Correct the error in the program using your text editor.
1. Compile the code using javac. (for help on how to do this, see https://introcs.cs.princeton.edu/java/15inout/windows-cmd.html)
1. Verify that the program executes. If it does not, keep searching for the error(s) in the file. 

## Step 6 - Update your local repo and push to Github

You will need to become familiar with a very common cycle of making changes to your local repository then pushing those changes back to Github where your instructor can review them and assign grades. Each time you make changes to your files, you will save them through your text editor (either through File->Save or Ctrl+S). This saves a copy of the changes you have made to your system, but have not saved them to your local repository or made them available online.

1. `git add .` This command will stage the changes you have made to the local repository
1. `git commit -m "commit message in quotations marks do not forget this"` This will commit staged changes to your local repository. Make sure to change the `"commit message in quotations marks do not forget this"` to some meaningful reminder about the changes you have made.
1. `git push` This will push committed changes from your local repository back to Github. Now your instructor can see them, and if you are working on a group project, your partner(s) can access them as well.

You should get used to using these commands frequently. Much of the challenge of developing complex software is learning to read error messages and feedback from the command line. If you type the command `git status` the command line will print out the current status of the repo. This will usually give you a clue for what you need to do next.

**Deliverable 4:** The corrected HelloWorld.java file pushed to the online repo.

#### *Note*: IntelliJ & Git
IntelliJ has Version Control System (VCS) capabilities built into it so that you can use the interface to directly interact with Github. It is recommended that you avoid using them until you are comfortable with the command line. 

## Step 7 - Online Delivery

Now that you have fixed a set of errors in the provided file, it is time to try and create your own Java class. In the same directory as the HelloWorld file, create a new file called `Menu.java`. Inside the file, create the same basic structure required by the HelloWorld class - a class header and a main method. 

The purpose of this class is relatively straightforward: it computes the amount owed on a restaurant order. When run, your system should:
1. Print a statement greeting the user in a friendly way with the name of one of your favorite restaurants to order from.
1. Display a list of five numbered items that are available for that restaurant and their price.
1. Prompt the user to enter the number of the item they want to order.
1. Calculate the tax on the item ordered at 6%.
1. Prompt the user for pickup or delivery. If delivery, add a $4.99 fee to the cost of the item ordered.
1. If the user picks delivery, prompt them for a tip: 0%, 10%, 15%, or 20%. The tip should be calculated using the base price of the item, not the item plus the fee.
1. Calculate the total cost and display it to the user. 
1. End the program.

All of the above should be contained in the main method. Do not try to write other methods at this time.

**Deliverable 5:** The working Menu.java file pushed to the online repo with the requested capabilities.

# Deliverables and Grading

| Weight | Deliverable                                                                                                           |
|--------|-----------------------------------------------------------------------------------------------------------------------|
| 15     | Modify this .md file so that your name and newly obtained Github profile name replaces the text.                      |
| 15     | In this directory, save a screenshot image showing what happens when you type `java` into your terminal/command line. |
| 15     | In this directory, save a screenshot image showing your installed IDE or text editor open. Then modify the statement. |
| 25     | The corrected HelloWorld.java file pushed to the online repo.                                                         |
| 30     | The working Menu.java file pushed to the online repo with the requested capabilities.                                 |

# Getting Stuck
There are times when you might get stuck on some part of an assignment. It happens to the best of us. If you need assistance on a specific part of your code, then be sure to try to `push` the most recent version of your files to Github. It makes it much easier for your instructor and TA to provide specific feedback on individual lines of code in the files that you submit. 
