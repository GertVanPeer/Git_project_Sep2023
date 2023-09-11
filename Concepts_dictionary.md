# My 1st Git project

- A Git repository is a single collection of documents for which you want to track the version (or timeline).

- GitHub is a collection of different repositories for which you want version control. Online.

# Conceptual areas

- Developping area: folder where the project is developped. It is on your computer (locally).

- Staging area: intermediate space to transfer from development area to your local repository. It is on your computer (locally).
  
  - staging is done by `$git add`
  - **Why is staging interesting?** To commit related changes (in different files), in the same commit.

- Local repository: The repository where you keep your snapshots. It is found in `.git `hidden folder. It is on your computer (locally).

P.S.: to check in what conceptual areas my files are, I can use `git status`

Testing what happens omitting `-m` in commit. It pops up an editor to force me to write a long message. The commit is automatically done upon saving and quiting.
