## Learning points (What, Why, How)
---
- What is version control? ( What is git? )
- Working Directory, Staging Area, Local Repository and Remote Repository.
- common Git commands ([Common terminal CLI commands]())


## Hands-on 
---
-  Create a Github Account.
-  Install Git in your env.
    ```bash 
    $ git --version   # check the version
    ```
-  [First-Time Git Setup](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)
    ```bash
    $ git config --global user.name "supergigi"
    $ git config --global user.email supergigi@example.com
    $ git config --list   # checking your settings
    ```
-  Initializing a Repository
    - Name: HelloWorld
    - Add File: README.md, hideme.md
    - Commit: my first commit
    - Branch: master
    - Add Ignoring Files（.gitignore): hideme.md
        ```bash
        $ git rm --cached "hideme.md"   
         ```

- View records (logs)
    ```bash
    $ git log
    $ git show {commit_id} 
    $ git log -p -HEAD  
    $ git log -p -{n}   # View the content of the last n commits
    $ git log --oneline --graph
    $ git log --oneline --author="Gigi|Trista"
    $ git log --oneline --grep="can you find me"
    $ git log --oneline --since="8am" --until="17pm"
    $ git blame -L 5,10 whoIsTheBadGuy.md
    ```
- branch
- tags
- Collaborating 


## Additional resources
---
- [Credential Storage](https://git-scm.com/book/en/v2/Git-Tools-Credential-Storage)
    ```bash 
    git config --global credential.helper cache   # the default is 15 minutes
    git config --global credential.helper store   # store credentials on disk
    git config --global credential.helper reset
    ```
- [Git Aliases](https://git-scm.com/book/en/v2/Git-Basics-Git-Aliases)
    ```bash 
    $ git config --global alias.co checkout
    $ git config --global alias.br branch
    $ git config --global alias.ci commit
    $ git config --global alias.st status
    ```

- [為你自己學Git 作者：高見龍](https://gitbook.tw/chapters/introduction/what-is-git)
