# gitWorkshop-THS
Introductory Git Version Control Workshop taught at Timberline High School for my Project-Based Instruction Class.

## Introduction
Hello, students! By now, you should have created your own Github account and registered for the Github Student Developer Pack. Congratulations! You've taken your first steps towards managing your code efficiently and becoming part of the open source community. Now, it's time to learn *how* to better manage your class codebase using Git.

## What is Git?
Git is what is known as version control software - it helps you manage your code by keeping track of its state over time, including additions, deletions, and changes. Github is a website that integrates with Git and functions a lot like Google Drive - but specifically for code. It lets you use the command line (or .zip files) to download your code, make changes, and save it on Github's servers, and serves as a backup if something happens to your files on your computer. A Git repository tracks all of the changes you make to your code, so that you can go back to a previous version of your project at any time! Having a copy of your code on Github's servers that you can access from anywhere also helps you manage your code across different computers efficiently. Professional coders and college students all over the world use Git to manage their code, and after this period you’ll have a valuable skill that will help you not only for the rest of AP CS, but for your whole coding career!


## Vocabulary Bank
* **Repository:** A project folder or collection of project folders connected to Git where you put your code files.
* **Local:** Something residing on your computer - in this case, the copy of your repository saved on your laptop!
* **Remote:** Something residing on someone else's computer - in this case, the repository on your Github account!
* **Commit:** Recording the changes to the code in your local repository to be saved in your remote repository.
* **Push:** Saving the commited changes to your local repository in your remote repository by "pushing" them up to Github's servers.
* **origin/master:** "origin" is your remote repository, and "master" is the main branch of your remote and local repository. A "branch" is a specific version of your repository, but we'll get to that later if we have time! For now, just know that "origin/master" is your remote repository (the one on your Github account) :)

## It's coding time!
### Forking a Repository

 1. Navigate to  [my Github repository for this lesson](https://github.com/lbosse/gitWorkshop-THS) (If you're reading my README you should already be here...).
 2. Click the "fork" button in the upper right hand corner of the screen. This will create your own personal copy of the repository in your account, where you can modify it freely without changing the code in my repository. This is often used when using someone else's code as a starting point for your own project or for proposing changes to their project. If you want to learn more about this after the lesson, check out [this page](https://help.github.com/articles/fork-a-repo/).
 3. You should now see your own copy of this repository on your Github profile page! Click on the repository name to go to it's page.
 4. You'll see a lot of buttons and options on this page! We'll get to those shortly. For now, click on the **"Clone or Download"** button and copy the link it gives you. You can also download it as a .zip file, but we're going to do things the cool way ;)
 
 ### Cloning a Repository to Your Computer
 1. Now that you've got the ".git" link to your repository, open up your terminal and navigate to the directory where you want to place your project folder. Once you're there, type this command into the terminal: `git clone https://github.com/lbosse/gitWorkshop-THS.git`.
 2. You're ready to start working!
 
 ### Committing to a Repository
 1. Open up the file `Greeting.java` with your favorite text editor and add the following method to the `Greeting` class: `public void sayHello() {
 System.out.println("Hello!"); }`
 2. Now, time for the good stuff! When we want to save, or "push" our code to our remote repository (the repository on Github where your code is stored), we first need to record our changes by "commiting" the changes we made to our code. This whole process takes four quick steps:
    1. Run the command `git status` in your project folder. This will show you both changes to "tracked" (files already being watched by git) and "untracked" (new) files. You should see the following message from this command:
    ``` 
    On branch master
    Your branch is up-to-date with 'origin/master'.
    Changes not staged for commit:
     (use "git add <file>..." to update what will be committed)
     (use "git checkout -- <file>..." to discard changes in working directory)
     	modified:   Greeting.java
     no changes added to commit (use "git add" and/or "git commit -a") 
    ```
   
   2. Add the changes you want to save to your commit by running `git add <file name>`. Do this for both modified and untracked files. Note that in coding directions, words inside angle brackets (< ... >) mean "fill in the blank with your file name, word, port, etc".
   3. Now, make your commit by running the command `git commit -m <message>` where "message" is a message describing the commit. These messages should be short (not much more than a sentence long) and describe what was accomplished with the commit. An example of a good commit message would be: "Made the greeting method in class Greeting static".
   4. You're finally ready to push your code to your Github repository! Run the command `git push origin master` to push the code. If you run `git status` again you'll get a message saying you're up-to-date with origin/master!
3. Congratulations! You've successfully updated your first Github repository :)
