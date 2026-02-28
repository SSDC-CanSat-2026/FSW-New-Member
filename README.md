# FSW-New-Member
New member project for FSW to learn about STM32 by having members write a snesor driver in SPI and then using the data to an XBEE radio in USART.

Made by **Sarah Tran** and **Joel Kubinsky**.


## What will you be doing?
You will be learning about understanding an existing Real-Time Operating Systems with the STM32. Afterwards, you will be writing driver code to translate sensor information to something that the STM32 can use. That information is then going to be sent to an XBEE radio to show on a Ground Control Station (which you do not need to code).

We will also be walking you through important code structures that will be important to understand before writing the driver code. If you do not care about it for some reason, you can skip to [here](#writing-driver-code-for-sensors).

### Requirements:
- Understanding of a programming language (ideally C or C++). This project is done in C.
- [STM32CubeIDE](https://www.st.com/en/development-tools/stm32cubeide.html) (use a guest account with your UFL email).
- Git and GitBash

**NOTE**: STM32CubeIDE's website can be a little slow sometimes, try asking your team lead if they have a version downloaded already. If not, try again later.

We are using an **STM32**G491​RCT6 (as of 2025-2026 CanSat) and so requires the STM32CubeIDE to automate a lot of the code! **When asked which version, just go with the newest.**

## Table of Contents
[1. Cloning and Making a Branch from GitHub](#part-1:-cloning-and-making-a-branch-off-of-github)

[2. Importing an STM32 project](#part-2-importing-an-stm32-project)

## PART 1: Cloning and Making a Branch from GitHub
#### Basic Linux Commands + Shortcuts that you should know.
Commands
- ls (Print what is in your current directory/folder)
- cd (Change Directory. Change your current directory/folder)

Shortcuts
- TAB key (The Command Line Interface, CLI, will try to autofill with what it has)


We will be doing this on the Command Line and then there will be an optional link with GitHub.

![GitHub Repo Homepage](Images/GitHubWebpage.png)
1. Click on the green "Code".

![Copy Repo Button](Images/GitHubCopy.png)
2. Then the copy icon.

3. Opening the GitBash terminal, go to the directory that you want to put the GitHub repo into. Then you would want to do:
```
git clone <link>
```
where \<link> will be what you just copied from GitHub. "Enter" to send the command. This makes a local version of the GitHub repository for you to access.

![CLI repo main branch](Images/MainBranchOnCLI.png)
4. Changing Directory to "FSW-New-Member", you should see that now you are on the "main" **branch**. A branch is like a version of the code and allows you to work independently from other people to work on something but then be able to **merge** branches together later on for collaboration. You DO NOT want to work on the main branch since you would want to make sure that your code works before having it be the definite version. A lot of repositories have restrictions that prevent you from sending new code to main, but that depends on group. We will now be making a new branch for you.

**Extra**: You are able to see other branches made by anyone by doing 
``` git branch ``` for local (on your computer branches) or ``` git branch -r ``` for branches by other users.

5. Make a new branch for this project by doing
```
git branch <name>
```
Replace \<name> with "\<FirstName>\_\<LastName>\_New_FSW_Project".

Now if you do ``` git branch ``` you should be able to see your new branch:
![Git with the new Branch](Images/GitBranches.png)

6. Move to that new branch by doing 
```
git checkout <name>
```
You should now see:
![Current Branch is the new Branch](Images/NewBranchCLI.png)

You are now able to open the project with an IDE like STM32CubeIDE and/or VSCode and start coding!

### Optional: Connecting your repo to GitHub Desktop application
Make sure you have done the instructions above for this. Also make sure that you are signed onto GitHub.

7. After opening GitHub desktop, click on this area to change repositories.
![GitHub Desktop HomePage](Images/GitHubDesktopStart.png)

Then `click "Add" => "Add existing repository..." => "Choose"` then find the folder for this project. You'll know when you are in it when you see a ```.git``` folder in the current directory. Now do `Select Folder => Add repository`  

You should be able to see now that your Repository is `FSW-New-Member` and the Current Branch to the right is the branch that you made.
![GitHub Deskstop Success](Images/GitHubDesktopCloneSuccess.png)


---
## PART 2: Importing an STM32 project
After opening a workspace, it should look something like this:
![STM32 Homescreen](Images/STM32Home.png)
On the top left corner, click "File" -> "Open Projects from File Systems".    

## Writing Driver Code for Sensors
SPI     - Reading ICM42688\
USART   - Writing to XBEEs

## Extra Resources
- Learn more about [SPI](https://youtu.be/MBwtJhO6b0I?si=Nb-yW6-bYA13eYJV) and [USART](https://youtu.be/fkVYkDuB_38?si=hZDJfQHnWz25cNov) from Dr. Schwartz here at UF.
  