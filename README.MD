# Git And GitHub Practical Assigment

## Introduction
In this Documantion We will perform some task on Git and GitHub for our understanding of Git and GitHub tools. 

### What is Git ?
Git is a free and open-source version control system. It helps developers track and manage changes to their source code over time. Using Git, 

You can:
-  Save versions (snapshots) of your project.
- Collaborate with others without overwriting each other’s work.
- Revert back to earlier versions if something breaks.
### What is GitHub

GitHub is a web-based platform built on top of Git. It allows developers to:
- Host and share their Git repositories online.
- Collaborate with others on code projects.
- Track issues, manage pull requests, and review code.

Store code in a secure and version-controlled environment.

It’s widely used by individuals and companies for open-source and private projects.

Here are the some task I'll done while learning the Git and GitHub

### TASk 1 : Create a New Repository on GitHub
- Name it:  git-practice-task
- Initialize with a README.md

### Output :
Prerequisites :
- GitHub account – For hosting repositories
- VS Code or any text editor – To write and manage your code
- Git – Version control system

Now that we have the prerequisites ready, let’s move ahead and start solving the task step-by-step.

1. First create one repository on GitHub.

![Project Screenshot](/Images/create%20Repo.png)

As you can see in above image 
first click on (+) symbol and click on "New Repository".

Now lets create one repository using below requiremnets:
1. Repository name : git-practice-task
2. Add README : On
3. Craete Repository.


Here is our First task is completed and our repository is created let's move to 2nd Task 


![project screenshot](/Images/repo.PNG)

### TASK 2 : Clone the Repository Locally
- git clone.
- Open The folder git-practice-task. 

### Output :
Lets start first to clone our repository on local machine. 

![project screenshot](/Images/clone%20repo.png)

Here you can see as 
1. Go to "Git-Practice-task"
2. click on code 
3. Copy the HTTP URL for cloning.

Open git in where you want to clone your repository.
```
git clone <paste-URl-HTTS-Of-Your-Repository>
```
Example :- 
```
git clone https://github.com/Vishu-Nargunde99/git-practice-task.git
```
![project screenshot](/Images/git%20clone.PNG)

You can check your repository on your local machine.
```
ls
```
![project screenshot](/Images/ls.png)

```
cd git-practice-task/
```
now you can open VS code through git.
```
code .
```
above cmd is use for open vs code through git 

Ok here is our 2nd task is completed.

### TASK 3 : Modify README.md on main
 - Add your name and course info to the file.
 - Stage and commit the changes.

First open the New Terminal for cmd actions.
![project screenshot](/Images/Terminal.png)

Now chnage the powershell to Git bash for easy GUI and Friendly terminal
![project screenshot](/Images/Git%20Bash.png)
here click on (+) sign and from drop down menu choose Git Bash.

- Now open the README.MD file and make chnages in it.
- save the file --> ctrl+s
- run the cmd for add file to remote repo 
    ```
    git add .
    ```
- Commit the chnages to repo.
    ```
    git commit -m "chnages done is Readme.md File"
    ```
- Push the chnages in Remote Repo.
    ```
    git push
    ```
![project screenshot](/Images/cmd.PNG)

Now you can check chnages done in your remote repo also. 

### TASK 4 :Create and Switch to a New Local Branch And Push New Branch to Remote
- Add a new file named "index.html"
- Add some sample HTML code in it.
- Stage and commit the file

First create on feature branch in main branch 
```
git checkout -b feature-A
```
git checkout -b cmd is use for create new brancha nd switch to that branch 

Create new file with name index.html
![project screenshot](/Images/newfile.png)

Add some code in index.html file and do some like 
```
git add .
git commit -m "chnages make in ndex.html file"
```
Push the new branch to main branch 
```
git push -u origin feature-A
```
Done Task 4.

### TASK 5 : Go to GitHub and Create a Pull Request
- Base branch: main
- Compare branch: feature-A
- Create the PR, but donʼt merge yet

Go to GitHub 
![project screenshot](/Images/compare%20&%20PR.PNG)
you can see there is one compare and pull request is pop-up

- click on "comapre & pull"
- Next click on "create pull request"
- here is our pull request created but don't merge it . 

### TASK 6 : Create Another Branch Locally
git checkout -b feature-B main
Modify the same index.html file with conflicting content (e.g.change the 
same lines).
Stage and commit the changes.
Push to remote and create a new pull request from **"feature-B"** to **"main"**.

Return to VS code terminal 
- create new branch with name **"feature-B"**.
    ```
    git checkout -b feature-B"
    ```
- Made chnages same line of index.html
- Add  the chnages of index.html
    ```
    git add .
    ```
- Commit the chnages.
    ```
    git commit -m "chnages made in index.html file for conflict check"
    ```
- Push the changes to remote-repo.
    ```
    git push -u origin feature-B
    ```
![project screenshot](/Images/feature-B.PNG)

Now check the Github there is "Comapre and pull" request is pup-up.

- Now go to GitHub and create pull reaquest of feature-B branch.

### TASK 7 :  Merge One PR First (feature-A-Merge)
- Merge feature-A pull request on GitHub.

Ok go to Github --> select repo --> click on "pull request" --> click on request from feature-A --> Merge the request. 

### TASk 8 : Now Try to Merge feature-B Pull Request.
- You will get a merge conflict.
- Follow the instructions to pull the latest changes and resolve the conflict

Got to GitHub --> select your repo --> click on pull request --> select PR from feature-B

Now when you have to merge is on notification is **"Resolve Conflict"**
![project screenshot](/Images/conflic.PNG)

### TASK 9 : Resolve the Conflict And Complete the Merge
- Open the file, remove conflict markers (<<<<<<< , ======= , >>>>>>> )
- Finalize the content
- Stage and commit the resolved file.
- Push the changes to 
- feature-B

Here is the how to solve conflicts.
- click on resolve conflicts 
- open this file 
    ![project screenshot](/Images/conflict%20file.PNG)
- Remove all (<<<<<, ======, >>>>>) symbol from that file. 
- Right-side-corner --> click on "mark as resolved"
- Now click on commit merge --> opens the pull request terminal --> click on " Merge pull request".

Done the Task.

## ✅ Summary
This Git assignment covers basic to intermediate Git operations. It includes creating a repository, working with branches (feature-A, feature-B), handling merge conflicts, and using pull requests. It helped me understand version control workflows and conflict resolution in real-time collaboration.



