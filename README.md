# A02
# Git, GitHub, and WebStorm Tutorial

## Part 1: Directions on Using WebStorm with Git and GitHub

### Step 1: Download and Install Required Software
To use Git with WebStorm, you need to install the following software:
- **[WebStorm](https://www.jetbrains.com/webstorm/download/)**
- **[Git](https://git-scm.com/downloads)**
- **[GitHub](https://github.com/)** (Sign up if you haven’t)

### Step 2: Configure Git in WebStorm
1. Open **WebStorm**.
2. Go to **File** > **Settings** (Windows/Linux) or **WebStorm** > **Preferences** (Mac).
3. Navigate to **Version Control** > **Git**.
4. Click **Test** to ensure Git is correctly installed.
5. Click **OK** to save settings.

### Step 3: Create a New Git Repository
1. Open WebStorm and create a new project.
2. Open **Terminal** inside WebStorm or use **VCS** > **Enable Version Control Integration**.
3. Run the command:
   ```sh
   git init
   ```
   This initializes a **Git repository** in the project folder.

### Step 4: Connect to GitHub
1. In WebStorm, go to **File** > **Settings** > **Version Control** > **GitHub**.
2. Click **Add Account** and log in using your GitHub credentials.
3. Click **Apply** and **OK**.

### Step 5: Create a Remote Repository on GitHub
1. Go to [GitHub](https://github.com/) and click the **New Repository** button.
2. Name the repository and set it to **public** or **private**.
3. Copy the repository URL.
4. In WebStorm, open **Terminal** and run:
   ```sh
   git remote add origin <repository_URL>
   ```

### Step 6: Basic Git Workflow
1. **Stage and commit changes**:
   ```sh
   git add .
   git commit -m "Initial commit"
   ```
2. **Push changes to GitHub**:
   ```sh
   git push -u origin main
   ```
3. **Fetch and pull updates from GitHub**:
   ```sh
   git fetch
   git pull origin main
   ```
4. **Create a new branch and switch to it**:
   ```sh
   git branch new-feature
   git checkout new-feature
   ```
5. **Merge branches**:
   ```sh
   git checkout main
   git merge new-feature
   ```

---

## Part 2: Glossary

- **Branch**: A separate version of a repository used for working on different features.
- **Clone**: A copy of a remote repository downloaded to a local machine.
- **Commit**: A saved change in a Git repository.
- **Fetch**: A command to retrieve the latest changes from a remote repository without merging them.
- **Git**: A distributed version control system that tracks changes in code.
- **GitHub**: A cloud-based platform for hosting Git repositories.
- **Merge**: Combining changes from different branches into a single branch.
- **Merge Conflict**: A situation when Git cannot automatically merge changes due to conflicting edits.
- **Push**: Sending committed changes from a local repository to a remote one.
- **Pull**: Fetching and merging changes from a remote repository to a local one.
- **Remote**: A repository stored on a hosting service like GitHub.
- **Repository**: A storage location for a project’s files and version history.

---

## References
- [JetBrains WebStorm Docs](https://www.jetbrains.com/help/webstorm/)
- [Git Documentation](https://git-scm.com/doc)
- [GitHub Docs](https://docs.github.com/en)

