# Instructions

In this assignment, you will familiarize yourself with two common **version control** workflows using **`git`** and **GitHub**: a **centralized workflow**; and a **forking workflow** (also known as the **"open source workflow"**).

With the centralized workflow, you will set up a **remote** repository on GitHub and a **local** **cloned** **repository** for your own project and practice **pushing** and **pulling** to/from this remote repository.

With the forking workflow, you will contribute to another student's project by **forking** their repository, making changes to your copy, and issuing a **pull request** to them to incorporate your changes.

Execute the following instructions in order.

## Before you get started

### Disclosure

Note that with version control systems such as `git`, it is easy to verify what work has or has not been done by whom on any project via the [log files](https://knowledge.kitchen/content/courses/software-engineering/slides/git-and-github/#logs). So activity using such systems cannot be faked (not that you would ever consider such a thing)!

### Download and install Git

Download and install `git` on your local machine, if you haven't already done so.

## Centralized workflow

In this part, we will try out a simple **centralized workflow**, where developers work with two copies of a repository: a **local** copy, where changes are made; and a **remote** copy, where completed changes are uploaded in order to be archived and shared with others.

### Create a remote GitHub repository

1.  Create an account on [GitHub](https://github.com), if you don't already have one.
2.  Create a new repository in your account on GitHub. If you are viewing this document in your own repository or a repository that has been created for you by **GitHub Classroom**, then this is already done!

### Create a local Git repository

1.  Clone your remote repository on GitHub to your own local machine.

2.  Create a `README.md` file in that directory using valid Markdown syntax. **Edit** this file such that it includes the following:
    - a link to an article or web site you find interesting related to software development/engineering (indirect relationships are ok)
    - a paragraph or two about what you find interesting about that article
    - remember that this will be public
    - Use Markdown syntax to make it look nice
3.  **Commit** your `README.md`` file to the local repository, including a meaningful commit message.

### Push changes to the upstream remote repository

1.  **Push** the latest version of the files in your local repository to the GitHub repository you created.
2.  Your two repositories should now be in-sync

### Share your repository with others

1.  Share the link to your GitHub repository on the course's Discord workspace and invite others to collaborate... they will do so via the **forking workflow** outlined below.

## Forking workflow

In this part, we will practice the **forking workflow**, also known as the **open source workflow**. Developers following this type of workflow interact with at least 3 different copies of a repository: the original **remote** repository that the developer ultimately intends to contribute to; a remote **clone** of that official repositor, known as a "`fork`"; and a local clone of the fork, where the developer makes changes.

### Find another repository to work with

1.  Wait for other students to also share their repository links from the centralized workflow part of this assignment.
2.  Select one of the other students' GitHub repository links that you find interesting.

### Fork that repository

1.  **Fork** that repository on GitHub - you now have a clone of that repository in your own GitHub account - we'll refer to this repository as "your forked repository"

### Make a local clone of that fork

1.  **Clone** your forked repository from GitHub to a new directory on your local machine (not the same directory as your original repository)

### Create a branch

1.  **Create a new branch** of your forked repository on your local machine where you will make changes to it. Switch to (i.e `checkout`) that branch.
2.  Edit the `README.md` file in your forked repository on your local machine to include a comment from you about that same article mentioned in the file. Make it looks nice using Markdown syntax.
    - Include your name in the edit you make, so we can clearly see who did it (we can also verify this with the Git change logs)
3.  Commit these changes to your local repository, including a meaningful commit message

### Push changes to your remote fork

1.  **Pull** any changes others may have made to the remote repository on GitHub while you were working (use the `--rebase` option on the git pull to put your own changes to the tip of the change history when merged)
2.  **Push** your changes to your remote repository on GitHub
3.  The branch you created with the changes you made will now be updated on your forked repository on GitHub

### Issue a pull request to the original repository

1.  [Make a pull request](https://help.github.com/articles/creating-a-pull-request/) on the other student's original repository from which you forked yours, asking them politely to include your changes in their original repository

### Accept contributions to your repository

1.  Make sure at least one other student has made a pull request with some changes to your own original repository - use Discord to coordinate this
2.  If the pull request changes you dislike, leave a response indicating why you have not accepted them, asking the other contributor to fix the problems
3.  Once you are happy with the changes, accept them
4.  Pull the updated files to the local repository of your project
5.  Merge any and all branches to the 'master' branch
6.  Commit any changes, including a meaningful commit message
7.  Push the result to the remote repository on GitHub
