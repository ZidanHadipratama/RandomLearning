# GitHub for Beginners 🚀

## Basic Git and GitHub Commands 💻

### GitHub Command List:
1. `git status`: Check the status of the code.

2. `git clone {{repository_url}}`: Clone a remote repository to your local machine.

3. `git add .`: Stage all changes for the next commit.

4. `git commit -m "{{commit_message}}"`: Commit changes with a descriptive message.

5. `git push`: Upload local commits to the remote repository.

6. `git checkout -b {{branch_name}}`: Create a new branch and switch to it.

7. `git merge {{branch_name}}`: Merge changes from a specific branch into the current branch.

8. `git pull origin {{branch_name}}`: Download and merge changes from a remote branch.

9. `git log`: View the commit history.

10. `git branch`: List all branches in the repository.

### GitHub Workflow - Starting a Project 🚀

1. **Create a Repository on GitHub** 🏁
   - Go to GitHub and click on "New" to create a new repository.
   - Enter a name for your repository, select public/private options, and choose to initialize with a README if needed.

2. **Clone the Repository** 📥
   ```bash
   git clone {{repository_url}}
   ```
   - Clone the newly created repository to your local project folder.

3. **Navigate to the Cloned Folder** 📂
   ```bash
   cd {{repository_folder}}
   ```
   - Move into the cloned repository directory.

4. **Start Coding** 🖥️
   - Begin working on your project by adding and modifying files.

   **Open the Folder in Visual Studio Code** 💡
   If you want to open the current folder in Visual Studio Code directly from the terminal, use the following command:

   ```bash
   code .
   ```

5. **Stage Changes** 📂
   ```bash
   git add .
   ```
   - Add the changes to the staging area before committing.

6. **Commit Changes** 📝
   ```bash
   git commit -m "{{commit_message}}"
   ```
   - Commit your changes with a descriptive commit message.

7. **Push to GitHub** 🚀
   ```bash
   git push
   ```
   - Upload the committed changes to your GitHub repository.

### GitHub Workflow - Uploading an Existing Project 🔄

1. **Create a Repository on GitHub** 🏁
   - Make a new repository on GitHub without initializing it with a README.

2. **Clone the Repository** 📥
   ```bash
   git clone {{repository_url}}
   ```
   - Clone the newly created repository to your local machine.

3. **Copy Existing Project** 📋
   - Copy and paste your existing project files into the cloned repository folder.

4. **Stage Changes** 📂
   ```bash
   git add .
   ```
   - Add the existing project files to the staging area.

5. **Commit Changes** 📝
   ```bash
   git commit -m "{{commit_message}}"
   ```
   - Commit the existing project files with a meaningful message.

6. **Push to GitHub** 🚀
   ```bash
   git push
   ```
   - Upload the existing project files to your GitHub repository.

### GitHub Workflow - Creating and Merging a New Feature 🚀

1. **Create a New Branch** 🌿
   ```bash
   git checkout -b {{branch_name}}
   ```
   - Create a new branch from the main project to work on the feature.

2. **Work on the New Feature** 💡
   - Implement and test the new feature or make necessary changes.

   **Open the Folder in Visual Studio Code** 🖥️
   To open the current folder in Visual Studio Code directly from the terminal, use the following command:

   ```bash
   code .
   ```

3. **Stage Changes** 📂
   ```bash
   git add .
   ```
   - Add the changes made for the new feature to the staging area.

4. **Commit Changes** 📝
   ```bash
   git commit -m "{{commit_message}}"
   ```
   - Commit the changes with a descriptive message.

5. **Merge with Main** 🔄
   ```bash
   git merge main
   ```
   - Merge the new feature branch with the main branch.

6. **Push Changes to GitHub** 🚀
   ```bash
   git push origin {{branch_name}}
   ```
   - Push the changes to the remote repository.

7. **Create a Pull Request** 🛎️
   - Go to your GitHub repository and click on "Pull Request."
   - Select the branches you want to merge and create the pull request.
   - Request a review from team members.

8. **Merge the Pull Request** 🤝
   - After approval, merge the pull request into the main branch on GitHub.

9. **Optional: Delete the Feature Branch** 🗑️
   ```bash
   git branch -d {{branch_name}}
   ```
   - If the feature branch is no longer needed, delete it.

## The Right GitHub Workflow 💡

### The Perfect Commit 💡

A crucial aspect

 of maintaining a clean and organized history in your Git repository is to create the perfect commit. The perfect commit involves:

- **Separate Different Topics into Individual Commits**: Each commit should focus on a specific topic or task. For example, if you fixed a bug and added a new feature, create separate commits for each change.

- **Give a Great Commit Message**:
   1. **Subject**: Provide a summary of what happened in the commit.
   2. **Body**: Include a more detailed explanation, such as what is now different than before, the reason for the change, and anything remarkable to watch out for.

### Branching Strategies 🌿

Before starting a project, it's essential to agree on a branching strategy suitable for your team and project. Defining a written convention will avoid mistakes and collisions. Consider the following points:

1. **Git Allows You to Create Branches**: However, it doesn't prescribe how to use them effectively. Therefore, have a written best practice on how your team will ideally structure work to avoid issues.

2. **Consider Your Team Size and Project Complexity**: The branching strategy should suit the size of your team, the complexity of your project, and how you handle releases.

It's crucial to onboard new team members with this information so they can quickly understand how your team collaborates using Git and GitHub.

### Pull Request 💡

A pull request is a mechanism on GitHub that allows you to propose changes to a repository and request that someone review and merge those changes into a branch of their choice. Pull requests are often used when working collaboratively on a project. The process involves the following steps:

1. Create a new branch from the main branch.
2. Make changes, commit them, and push the branch to the remote repository.
3. Go to the repository on GitHub and create a pull request, specifying the source branch and target branch for the merge.
4. Request a review from team members or collaborators.
5. Discuss the changes, make necessary adjustments, and address any feedback.
6. After approval, merge the pull request into the target branch, and the changes are now part of the project.

### Merge Conflicts 💡

Merge conflicts occur when integrating commits from different sources, and there are contradictory changes in the same lines of code or when using certain Git commands like `git merge`, `git rebase`, `git pull`, `git cherry-pick`, and `git stash apply`.

When a merge conflict occurs, Git cannot automatically resolve the differences, and it requires human intervention to determine how to proceed. Here's how to handle merge conflicts using Visual Studio Code:

1. **Identify the Conflict**: When you attempt to merge or pull changes from a remote branch into your current branch, and a conflict occurs, Visual Studio Code will display a notification in the source control tab. Click on the notification to see a list of files with conflicts.

2. **Open the Conflicting File**: Click on one of the conflicted files to open it in the editor. You'll see the conflict markers indicating the conflicting sections in the file.

3. **Resolve the Conflict**: Carefully review the conflicting sections and decide which changes to keep. You can manually edit the file to remove the conflict markers and choose the desired content. For example, you might keep both changes or choose one over the other.

4. **Save the File**: After resolving the conflict, save the file.

5. **Stage the Resolved Changes**: Use the source control tab in Visual Studio Code to stage the resolved changes. Click on the "+" icon next to the file name to stage the changes for commit.

6. **Commit the Merge**: With the conflicts resolved and changes staged, click on the checkmark icon (✓) in the source control tab to commit the merge. Provide a meaningful commit message that explains the changes you made to resolve the conflict.

7. **Push the Changes**: After committing the merge, you can push the changes to the remote repository by clicking on the "Sync" icon in the bottom-left corner of Visual Studio Code.
