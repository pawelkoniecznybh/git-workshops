### Hands-On Exercises

**Exercise 1: Creating a Branch, Adding a File, Commit, and Pull Request**

-   **Step 1: Create a Branch with Your Name**
    -   Open your terminal (Terminal, Git Bash, or PowerShell) in the cloned `git-workshops` repository directory.
    -   You have to specify git email and username, to do that:
        -   `git config user.name “your-github-username”`
        -   `git config user.email "your-github-account-email@gmail.com"`
    -   Navigate to main branch `git checkout main`
    -   Using the command `git checkout -b [your-name]`, create a new branch. Replace `[your-name]` with your actual name.
        -   _Example:_ If your name is John, use the command: `git checkout -b john`
    -   **Explanation:** This command creates a new branch and immediately switches to it (`checkout`). This branch is your personal workspace.
-   **Step 2: Add a File with Your Name**
    -   Ensure you are in the main directory of the repository.
    -   Create a new text file named `[your-name].py`. Again, replace `[your-name]` with your actual name.
        -   _Example:_ If your name is John, create a file `john.py`.
    -   Open the file `[your-name].py` in Visual Studio Code.
    -   In the file, type a single line of code: `print("Your Name")`. Replace "Your Name" with your actual name.
        -   _Example:_ In the file `john.py` type: `print("John")`
    -   Save the file.
-   **Step 3: Add and Commit Changes**
    -   In the terminal, use the command `git add .` to add the new file to the staging area.
        -   _Example:_ `git add .`
    -   Next, commit the changes with a description. Use the command `git commit -m "Add file [your-name].py"`, replacing `[your-name].py` with your file name.
        -   _Example:_ `git commit -m "Add file john.py"`
    -   **Explanation:** `git add` prepares the file for commit, and `git commit` saves the changes to the repository history. A good commit message is important to understand what was changed.
-   **Step 4: Push the Branch to the Remote Repository (Push)**
    -   Use the command `git push origin [your-name]` to push your local branch to the remote GitHub repository.
        -   _Example:_ `git push origin john`
    -   **Explanation:** `origin` is an alias for the remote repository, and `[your-name]` is the name of your branch. This command makes your changes available on GitHub.
-   **Step 5: Create a Pull Request on GitHub**
    -   Open a web browser and navigate to the `git-workshops` repository on GitHub.
    -   GitHub should display a message about the pushed branch and ask if you want to create a Pull Request. Click the "Compare & pull request" button.
    -   Click "Create pull request".
    -   **Explanation:** A Pull Request is a proposal to merge your changes into the main branch (`main`). It’s a way to start the code review and merging process.
-   **Step 6: Merge Your Changes to the `main` Branch**
    -   Click “Merge pull request”
-   **Step 7: Update Local `main` Branch and Download Changes (Pull)**
    -   Return to Visual Studio Code and the terminal.
    -   Switch to the `main` branch using the command: `git checkout main`
    -   Download the latest changes from the remote `main` branch using the command: `git pull origin main`
    -   Now your local `main` branch should contain the file you added and the files added by other participants.

**Exercise 2: Simulating and Resolving a Merge Conflict**

-   Follow along with the instructor's demonstration on simulating a merge conflict.
-   Learn the steps to resolve conflicts using merge tools in VS Code.
