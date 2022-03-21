# Installing Git

1. Download Git from [here](https://git-scm.com/download)
2. Run the installer
3. Open command prompt
4. Run `git config --global user.name "YOUR_NAME"`
    - You should use your real name (at least for FRC)
5. Run `git config --global user.email "YOUR_EMAIL"`
    - You should use the email you used for GitHub (at least for FRC)

# Downloading Code from GitHub

1. In the selected repository, click the Code dropdown, and copy the HTTPS URL
2. In the folder, you want to create a subfolder with the repository, open command prompt and run `git clone URL_FROM_STEP_1`
    - On Windows, you can open command prompt by clicking the file path bar (left of search), typing `cmd`, and pressing Enter
    - Git creates a subdirectory like the following:
      ```
      └───Documents [git clone https://github.com/roboticsmgci/main.git]
          └───main
              ├───guides
              ├───.gitignore
              └───README.md
      ```

# Uploading Code to GitHub

Uploading is more formally called *pushing*. 

1. Open command prompt in the folder
2. Run `git add .`
3. Run `git commit -m "MESSAGE"`
    - Make sure you have an informative message
4. Run `git push`

This part is a simplified tutorial. There are many more commands and components you should know. Please research these:
 - `.gitignore` file
 - Branching and forking
 - Pull requests and GitHub issues
 - Merging and merge conflicts
 - Using Git and GitHub in your preferred IDE
