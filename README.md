# Git-Cheat-Sheet

>  Click ⭐ if you like the project. Pull Request are highly appreciated. Follow me [@sisitarak](https://www.linkedin.com/in/sisitarak/) for technical updates.



### Table-of-Contents
<details open>
<summary>
Hide/Show table of contents
</summary>

| No. | Topics                                                                                                                                                                                                     |
| --- | -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| 1   | [What is Git?](#what-is-git)                                                                                                                                                                               |
| 2   | [What is GitHub?](#What-is-github)                                                                                                                                                                         |
|     | **Cheat Sheet with Commands**                                                                                                                                                                              |
| 3   | [What is Git Cheat Sheet?](#what-is-git-cheat-sheet)                                                                                                                                                       |
| 4   | [Disclaimer](#disclaimer)                                                                                                                                                                                  |



1.  ### What is Git?

    Git is the free and open source distributed version control system that's responsible for everything GitHub related that happens locally on your computer. This cheat sheet features the most important and commonly
    used Git commands for easy reference.

    **[⬆ Back to Top](#table-of-contents)**



2. ### What is GitHub?

   GitHub is a web-based platform used for version control and collaboration on projects primarily based on Git. It offers a range of features including source code management (version control), issue tracking, pull
   requests, code review, and project management tools.

   GitHub is widely used by developers and teams for
       - managing and sharing code,
       - collaborating on projects, and
       - contributing to open-source software.

   **[⬆ Back to Top](#table-of-contents)**



3. ### What is Git Cheat Sheet?

   ** SETUP **

   Configuring user information used across all local repositories
   
       '''bash
   

       # set a name that is identifiable for credit when review version history
       git config --global user.name “[firstname lastname]”
   
     
       # set an email address that will be associated with each history marker
       git config --global user.email “[valid-email]”
   

       # set automatic command line coloring for Git for easy reviewing
       git config --global color.ui auto
   

       '''


    ** INIT **

    Configuring user information, initializing and cloning repositories

       '''bash


       # initialize an existing directory as a Git repository
       git init
   

       # retrieve an entire repository from a hosted location via URL
       git clone [url]


       '''


    ** STAGE & SNAPSHOT**

   Working with snapshots and the Git staging area

       '''bash


       # show modified files in working directory, staged for your next commit
       git status
   

       # add a file as it looks now to your next commit (stage)
       git add [file]
   

       # unstage a file while retaining the changes in working directory
       git reset [file]
   

       # diff of what is changed but not staged
       git diff
   

       # diff of what is staged but not yet committed
       git diff --staged
   

       # commit your staged content as a new commit snapshot
       git commit -m “[descriptive message]”


       '''
   

    ** BRANCH & MERGE **

   Isolating work in branches, changing context, and integrating changes

       '''bash


       # list your branches. a * will appear next to the currently active branch
       git branch
   

       # create a new branch at the current commit
       git branch [branch-name]
   

       # switch to another branch and check it out into your working directory
       git checkout
   

       # merge the specified branch’s history into the current one
       git merge [branch]
   

       # show all commits in the current branch’s history
       git log


       '''


    ** INSPECT & COMPARE **

   Examining logs, diffs and object information

       '''bash


       # show the commit history for the currently active branch
       git log
   

       # show the commits on branchA that are not on branchB
       git log branchB..branchA
   

       # show the commits that changed file, even across renames
       git log --follow [file]
   

       # show the diff of what is in branchA that is not in branchB
       git diff branchB...branchA
   

       # show any object in Git in human-readable format
       git show [SHA]


       '''
   

   ** TRACKING PATH CHANGES **

   Versioning file removes and path changes

       '''bash


       # delete the file from project and stage the removal for commit
       git rm [file]
   

       # change an existing file path and stage the move
       git mv [existing-path] [new-path]
   

       # show all commit logs with indication of any paths that moved
       git log --stat -M
   

       '''
   

   ** IGNORING PATTERNS **

   Preventing unintentional staging or commiting of files

       '''bash


       # system wide ignore pattern for all local repositories
       git config --global core.excludesfile [file]
   

       # Save a file with desired patterns as .gitignore with either direct string matches or wildcard globs.
       logs/
       *.notes
       pattern*/


       '''
   

   ** SHARE & UPDATE **

   Retrieving updates from another repository and updating local repos

       '''bash


       # add a git URL as an alias
       git remote add [alias] [url]
   

       # fetch down all the branches from that Git remote
       git fetch [alias]
   

       # merge a remote branch into your current branch to bring it up to date
       git merge [alias]/[branch]
   

       # Transmit local branch commits to the remote repository branch
       git push [alias] [branch]
   

       # fetch and merge any commits from the tracking remote branch
       git pull


       '''
   

   ** REWRITE HISTORY **

   Rewriting branches, updating commits and clearing history

       '''bash


       # apply any commits of current branch ahead of specified one
       git rebase [branch]
   

       # clear staging area, rewrite working tree from specified commit
       git reset --hard [commit]

     
       '''
   

   ** TEMPORARY COMMITS **

   Temporarily store modified, tracked files in order to change branches

       '''bash


       # Save modified and staged changes
       git stash
   

       # list stack-order of stashed file changes
       git stash list
   
   
       # write working from top of stash stack
       git stash pop
   

       # discard the changes from top of stash stack
       git stash drop


       '''
   
   
   **[⬆ Back to Top](#table-of-contents)**



4. ### Disclaimer

   ** Note: **

    This Git cheat sheet is provided for basic informational purposes only. While we strive to ensure the accuracy and reliability of the information presented here, it is important to note that Git commands and workflows may vary based on factors such as operating         system, Git version, and individual project requirements.

    Before executing any Git commands, we strongly recommend reviewing the official Git documentation and exercising caution, especially when working with sensitive or production-level repositories. Additionally, always make sure to back up your data and verify the         impact of any commands on your repository before proceeding.
    
    By using this Git cheat sheet, you acknowledge and agree that the authors and contributors are not liable for any damages or losses resulting from the use or misuse of the information provided herein.

    Good luck and Pull Request are highly appreciated 😊
