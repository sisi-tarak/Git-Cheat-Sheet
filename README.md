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
|     | **Cheat Sheet**                                                                                                                                                                                            |
| 3   | [What is Git Cheat Sheet?](#what-is-git-cheat-sheet)                                                                                                                                                       |
| 4   | [What are Git Commands?](#What-are-git-commands)                                                                                                                                                           |



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



3. ### What are Git Cheat Sheet?

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


    ** STAGE **

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
   

   **[⬆ Back to Top](#table-of-contents)**



5. ### What are Git init Commands?
