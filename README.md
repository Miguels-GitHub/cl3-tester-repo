# cl3-tester-repo

## Introduction
Hello, CL3 MSSA!  I've created this GitHub repository for you to get some hands-on practice making code changes in a version control system, so you don't have to worry about breaking anyone's actual project ;)  Follow the steps below to begin!

## Getting Started
This tutorial assumes that you've already done the following:
1. Learned some of the basics of Git commands
2. Installed Git bash or plan to use some other tool (such as the Visual Studio/VSCode UI) to make and push your changes

To contribute to the project and make a change, follow these steps:
1. Fork my GitHub repository.
2. Clone your fork (the one in your GitHub account) to a directory on your local machine.
3. Open up the project in whatever tool you're using for your Git operations.
    * Command line: (Git bash), navigate to the directory containing your local repository that you cloned on your machine.
    * Visual Studio: open the project using the .sln file in the top-level directory.
    * VSCode: open the top-level folder containing all of the files in the repository.
3. Create a new branch from "master".
    * Note: Branch names usually summarize whatever change it is you're making in that branch.  In this case, you'll simply be adding your name to a list, so you can name it something simple like `add-my-name`.
    * Command line: `git checkout -b <your branch name>` -> creates and checks out the new branch at the same time.
    * Visual Studio: go to Team Explorer -> Branches -> Right-click "master" -> "New local branch from..."
    * VSCode: Ctrl+Shift+P, in the bar at the top type "Git create branch" and select that option.  Enter a branch name and hit "Enter."  When it asks you to "Select a ref to create the new branch from" pick "master."
    * Note: At any time, you can view the branch that you're currently on, as well as all the other branches you've created, by typing "git branch" in your command line/terminal.
5. If you haven't already, open the project in your code editor, and...make your changes!  We'll keep it simple to start - just add your name with a message to the "Program.cs" file.
    * Note: Make sure to run the program after any changes you  make and before committing/pushing, to make sure it still works.  Normally you'd perform tests and checks when the code gets pushed, but we're starting simple - just test on your own for now :)
6. Commit your changes.
    * Command line: `git status` to view the files you've changed. `git add <filepath>` for each file you want to submit your changes for (or `git add --all` as a shortcut if you want to commit all the changes you've made).  `git commit -m "<commit message briefly explaining the changes you made>`.
    * Visual Studio: Team Explorer -> Changes -> Click the plus sign to "stage" all your changes for commit (or right-click the files you want to stage and add them individually).  Enter a commit message in the box explaining the changes you  made, and then hit the "Commit" button.
    * VSCode: Click the little branch-y icon on the left panel (probably has a blue circle with a number on it by this point).  Click the plus sign to the right of each file you want to submit your changes for.  Enter a message in the box explaining the changes you made, then hit Ctrl+Enter to commit.
7. Push your changes.  This takes the changes you've made to the project on your local machine (your origin), and pushes them to an online branch of the fork you created in your GitHub repository online (your remote).
    * Note: More likely than not, you'll receive some type of error saying that you don't have a remote branch set up yet to track your local branch.  If this happens, most of the tools are pretty good about walking you through how to set this up - just follow the instructions.
    * Ultimately what we want is to have your local branch containing your code changes (origin/branch-you-created) match an online counterpart with the same name in your GitHub repository (remote/branch-you-created).
    * Once you have your remote branch set up to track your local branch, each of the tools has a way to "push" the changes from your local project to your GitHub repository.
    * Command line: "git push" should be sufficient.  If the prompt needs any additional information it will tell you.
    * Visual Studio: Team Explorer -> Sync -> Under "Outgoing Commits" click on "push".
    * VSCode: In the same panel where you did your commit, click the three little dots in the upper right corner and hit "push."  I've never used this method personally but I assume it works.
8. Almost done!  Finally, go into GitHub and create your pull request for your changes.
    * If you go to your fork of my repository in your GitHub account, often there will be a notification bar at the top showing the changes you just made, and it usually includes a link to create a pull request.  If not, there's a "pull request" button right below the green "Clone or download" button.
    * The base repository (the first box) should be set to my repository (ackaufman/cl3-tester-repo), with base: master.  The head repository should be set to your fork (<your-github-username>/cl3-tester-repo), with compare: <the branch you made your changes in>.
    * If there are any other fields to fill out, do so as needed, then hit "Create pull request."  What we're doing here is requesting to pull - or merge - your code changes into the main repository for the project (often called the canonical master).
    * Note that I've got the repository set up such that you can't merge your own changes automatically - at least one other person has to do a code review for you and approve them!
9. From what I've seen, most of the time it's common practice to wait for the owner of the repository to hit the final button to approve and merge your code changes - then your pull request is considered "complete" and your code should show up in my repository!
10. Git problems happen...a lot.  If you run into errors that aren't clearly explained by the Git tool you're using, you can try to look up how to fix them, or ask someone with some Git experience to help you.
    * Merge conflicts occur when you and someone else both modified the same line of code in different ways, and you're trying to merge your version of the file together with theirs.  Resolving merge conflicts is not easy but definitely doable, and there are plenty of tools that can help.  For now, if you run into this let me know and we can work through it together.
    * The best way to avoid merge conflicts is to do a "git pull" from the master of the original repository (mine, in this case) immediately before each time you open up the project to work on it.  This takes any changes that have been merged into the canonical master since your last pull and merges them into your working branch, so you are always basing your changes off the most updated version of the code.

## Conclusion
Let me know if you need any help with any of the steps above - I use a mix of different Git tools depending on the situation, so a few areas are a little ambiguous.  Hopefully all goes well and I start seeing some forks and pull requests soon!