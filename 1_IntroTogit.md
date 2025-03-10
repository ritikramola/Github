# Introduction

Imagine you're a new software developer at a firm that writes avionics software for commercial airliners. Quality control is critical, and developers work in small teams using Git for version control. You've heard of version control, but you've never used Git, so you're eager to catch up!

You decide to build a website that lets you and your friends share pictures of your cats, so you can learn Git in a fun environment before bringing that knowledge to work. You set out to build the site by using Git to keep track of changes and keep all the source code files backed up in case the server goes down. But before diving head-first into Git, you must cover the basics

In this module, you'll get an introduction to version control, and Git. Git can seem a little cryptic at first, and it can even be frustrating at times. But if you learn it step by step, you'll find that there's a reason Git is quickly becoming the world's most popular version control system—not just for software developers, but also for teams that write documentation and collaborate on other work.

## What is version control?

A version control system (VCS) is a program or set of programs that tracks changes to a collection of files. One goal of a VCS is to easily recall earlier versions of individual files or of the entire project. Another goal is to allow several team members to work on a project, even on the same files, at the same time without affecting each other's work.

Another name for a VCS is a software configuration management (SCM) system. echnically, version control is just one of the practices involved in SCM. A VCS can be used for projects other than software, including books and online tutorials.

**With a VCS, you can:**

See all the changes made to your project, when the changes were made, and who made them.

Include a message with each change to explain the reasoning behind it.

Retrieve past versions of the entire project or of individual files.

Create branches, where changes can be made experimentally. This feature allows several different sets of changes (for example, features or bug fixes) to be worked on at the same time, possibly by different people, without affecting the main branch. Later, you can merge the changes you want to keep back into the main branch.

Attach a tag to a version—for example, to mark a new release.

### Distributed version control
Earlier instances of VCSes, including CVS, Subversion (SVN), and Perforce, used a centralized server to store a project's history. This centralization meant that the one server was also potentially a single point of failure.

Git is distributed, which means that a project's complete history is stored both on the client and on the server. You can edit files without a network connection, check them in locally, and sync with the server when a connection becomes available. If a server goes down, you still have a local copy of the project. Technically, you don't even have to have a server. Changes could be passed around in e-mail or shared by using removable media, but no one uses Git this way in practice.

### Git terminology
To understand Git, you have to understand the terminology. Here's a short list of terms that Git users frequently use.

**Working tree**: The set of nested directories and files that contain the project that's being worked on.

**Repository (repo)**: The directory, located at the top level of a working tree, where Git keeps all the history and metadata for a project. Repositories are almost always referred to as repos. A bare repository is one that isn't part of a working tree; it's used for sharing or backup. A bare repo is usually a directory with a name that ends in 
*.git*—for example, project.git.

**Hash**: A number produced by a hash function that represents the contents of a file or another object as a fixed number of digits. Git uses hashes that are 160 bits long. One advantage to using hashes is that Git can tell whether a file has changed by hashing its contents and comparing the result to the previous hash. If the file time-and-date stamp is changed, but the file hash isn’t changed, Git knows the file contents aren’t changed.

**Object**: A Git repo contains four types of objects, each uniquely identified by an SHA-1 hash. A *blob object* contains an ordinary file. A *tree object* represents a directory; it contains names, hashes, and permissions. A *commit object* represents a specific version of the working tree. A tag is a name attached to a commit.

**Commit**: When used as a verb, commit means to make a commit object. This action takes its name from commits to a database. It means you are committing the changes you have made so that others can eventually see them, too.

**Branch**: A branch is a named series of linked commits. The most recent commit on a branch is called the *head*. The default branch, which is created when you initialize a repository, is called *main*, often named master in Git. The head of the current branch is named *HEAD*. Branches are an incredibly useful feature of Git because they allow developers to work independently (or together) in branches and later merge their changes into the default branch.

**Remote**: A remote is a named reference to another Git repository. When you create a repo, Git creates a remote named *origin* that is the default remote for push and pull operations.

Commands, subcommands, and options: Git operations are performed by using commands like *git push* and *git pull.* git is the command, and push or pull is the subcommand. The subcommand specifies the operation you want Git to perform. Commands frequently are accompanied by options, which use hyphens (-) or double hyphens (--). For example, *git reset --hard*.

These terms and others, like push and pull, will make more sense shortly. But you have to start somewhere, and you might find it helpful to come back and review this glossary of terms after you finish the module.

### The Git command line
Several different GUIs are available for Git, including GitHub Desktop. Many programming editors, like Microsoft Visual Studio Code, also have an interface to Git. They all work differently and they have different limitations. None of them implement all of Git's functionality.

### Git and GitHub
As you work with Git, you might wonder about differences between the features it offers and the features offered on GitHub.

As mentioned earlier, Git is a distributed version control system (DVCS) that multiple developers and other contributors can use to work on a project. It provides a way to work with one or more local branches and then push them to a remote repository.

GitHub is a cloud platform that uses Git as its core technology. GitHub simplifies the process of collaborating on projects and provides a website, more command-line tools, and overall flow that developers and users can use to work together. GitHub acts as the remote repository mentioned earlier.

#### Key features provided by GitHub include:

Issues
Discussions
Pull requests
Notifications
Labels
Actions
Forks
Projects

## Exercise

### Configure Git
1.In Cloud Shell, to double-check that Git is installed, type git --version:

    git --version

2.You should see output that looks something like this example:

    Output
    git version 2.7.4

3.To configure Git, you must define some global variables: user.name and user.email. Both are required for you to make commits.

4.Set your name in Cloud Shell with the following command. Replace <USER_NAME> with the user name you want to use.
    git config --global user.name "<USER_NAME>"

5.Now, use this command to create a user.email configuration variable, replacing <USER_EMAIL> with your e-mail address:
    git config --global user.email "<USER_EMAIL>"

6.Run the following command to check that your changes worked:
    git config --list

7.Confirm that the output includes two lines that are similar to the following example. Your name and e-mail address will be different from what's shown in the example.

Output
user.name=User Name
user.email=user-name@contoso.com

### Set up your Git repository
Git works by checking for changes to files within a certain folder. We'll create a folder to serve as our working tree (project directory) and let Git know about it, so it can start tracking changes. We tell Git to start tracking changes by initializing a Git repository into that folder.

Start by creating an empty folder for your project, and then initialize a Git repository inside it.

1.Create a folder named Cats. This folder will be the project directory, also called the working tree. The project directory is where all files related to your project are stored. In this exercise, it's where your website and the files that create the website and its contents are stored.
    mkdir Cats

2.Change to the project directory by using the cd command:
    cd Cats

3.Now, initialize your new repository and set the name of the default branch to main:

If you're running Git version 2.28.0 or later, use the following command:
    git init --initial-branch=main

Or use the following command:
    git init -b main

After you run the initialize command, you should see output that's similar to this example:

Output
    Initialized empty Git repository in /home/<user>/Cats/.git/
    Switched to a new branch 'main'

Now, use a git status command to show the status of the working tree:
    git status

Use an ls command to show the contents of the working tree:
    ls -a

## Basic Commands
Git works by remembering the changes to your files as if it's taking snapshots of your file system.

### git status
The first and most commonly used Git command is *git status*. You've already used it once, in the preceding exercise, to see that you had initialized your Git repo properly.

*git status* displays the state of the working tree (and of the staging area—we'll talk more about the staging area soon). It lets you see which changes are currently being tracked by Git, so you can decide whether you want to ask Git to take another snapshot.

### git add
*git add* is the command you use to tell Git to start keeping track of changes in certain files.

The technical term is staging these changes. You'll use git add to stage changes to prepare for a commit. All changes in files that have been added but not yet committed are stored in the staging area.

### git commit
After you've staged some changes for commit, you can save your work to a snapshot by invoking the *git commit* command.

Commit is both a verb and a noun. It has essentially the same meaning as when you commit to a plan or commit a change to a database. As a verb, committing changes means you put a copy (of the file, directory, or other "stuff") in the repository as a new version. As a noun, a commit is the small chunk of data that gives the changes you committed a unique identity. The data that's saved in a commit includes the author's name and e-mail address, the date, comments about what you did (and why), an optional digital signature, and the unique identifier of the preceding commit.

### git log
The *git log* command allows you to see information about previous commits. Each commit has a message attached to it (a commit message), and the *git log* command prints information about the most recent commits, like their time stamp, the author, and a commit message. This command helps you keep track of what you've been doing and what changes have been saved.

### git help
You've already tried out the *git help* command, but it's worth reminding you about. Use this command to easily get information about all the commands you've learned so far, and more.

Remember, each command comes with its own help page, too. You can find these help pages by typing *git <command> --help*. For example, *git commit --help* brings up a page that tells you more about the git commit command and how to use it.

