# Git and Version Control Cheatsheet 📜

Git is a version control system, providing a way to track changes in code and collaborate with others. It helps manage the history of your code, allowing you to revert changes, collaborate with other developers, and maintain different versions of your project. 🚀💻

### 📘 Terms:

- **Directory:** Also known as a folder, it is a location on your computer where files are stored. 📂
- **Terminal:** A command-line interface (CLI) for executing text commands. 💻
- **CD:** Stands for "Change Directory," used to navigate through folders in the terminal. 🔄
- **Code Editor:** A text editor designed for writing and editing code. 📝
- **Repository:** Also known as a project, it is a folder where your project is kept. 🗃️
- **GitHub:** A website to host and manage Git repositories. 🌐

### 💻 Git Commands:

- **`git --version`**: Check if Git is installed on your machine. ✨
- **`git clone {{Clone with SSH}}`**: Clone a repository from GitHub to your local machine. 📥
- **`git status`**: Show the status of the files in your repository. 📊
- **`git add .`**: Track all changes in your repository. ➕
- **`git add {{file name}}`**: Track specific changes or individual files. ➕
- **`git commit -m {{Title message}} -m {{Description message}}`**: Save files with a commit message. 💾
- **`git push origin {{Branch name (usually master)}}`**: Upload commits to GitHub. 🚀
- **`git pull`**: Download changes from the remote repository to your local machine. 📥

### 🔗 Connecting Local Machine to GitHub:

1. Generate an SSH key with `ssh-keygen`. 🔑
2. Copy the contents of the `.pub` file and add it to the SSH and GPG keys in GitHub settings. 🔍

### :octocat: Creating a New Repository:

1. Create a new folder. 📂
2. Run `git init` to initialize a new Git repository. 🚀
3. Add and commit your files. ➕
4. Add a remote repository with `git remote add origin {{SSH URL}}`. 📥
5. Push your code to the remote repository with `git push origin master`. 🚀

### 🔀 Git Branching:

- **`git branch`**: Show all branches and the current branch. 🌿
- **`git checkout`**: Switch between branches. 🔄
- **`git checkout -b {{New Branch Name}}`**: Create a new branch and switch to it. ➕
- **`git diff {{New Branch Name}}`**: Show differences between branches. 👁️
- **`git merge {{New Branch Name}}`**: Merge changes from another branch. 🔄
- **`git push --set-upstream origin {{New Branch Name}}`**: Push a new branch to GitHub. 🚀

### 🚢 Pull Request:

- Pull Request (PR) is a request to pull your code into another branch. 📥
- After making changes on a branch, create a PR on GitHub. 📥

### ⚠️ Merge Conflict:

- Occurs when merging two branches with conflicting changes. ⚠️
- Use a code editor to resolve conflicts. 📝
- Commit changes after resolving conflicts. 💾

### ⏪ Undoing in Git:

- **`git reset HEAD`**: Undo the most recent commit. ⏪
- **`git reset HEAD~1`**: Undo the last commit. ⏪
- **`git log`**: View commit history. 📜
- **`git reset {{hash}}`**: Reset to a specific commit. ⏪
- **`git reset --hard {{hash}}`**: Reset and discard changes. ⏪

🌟 Keep on coding and collaborating with Git! Happy coding! 🚀🎉
