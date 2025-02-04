# GitHub Training By Aman Sir

## Git and GitHub
Git is the version control software that can help you keep a history of your commits and features that you make in code. On the other hand GitHub is something that facilitates and allows for that functionality.

## Git Installation Steps
#### For Windows

1. Download the [latest version of Git](https://git-scm.com/download/win) and then run the installation with Administrator Rights.
2. Choose an appropriate installation location (default is fine).
3. Install the default components, including Git GUI and Git Bash.
4. Choose your preferred Git default editor. (Sublime Text, VSCode or Notepad++ should be more than fine).
5. Add Git to the Windows PATH.
6. Accept the default line ending conversion for Unix and Windows compatibility.
7. Chose the extra option to enable system caching.
8. Click Finish to complete the install.
9. Open powershell and type git --version to confirm installation.

## Configure Git and GitHub

#### Step 1: Create a GitHub account

 - Go to [GitHub.com](https://github.com/) and create an account! During the account setup, it will ask you for an email address. This needs to be a real email, and will be used by default to identify your contributions. If you are privacy conscious, or just don’t want your email address to be publicly available, make sure you tick the following two boxes on the [Email Settings](https://github.com/settings/emails) page after you have signed in.

#### Step 2: Create a Personal Access Token 
 - [Folow step 2 of Configure Git and GitHub](./assests/GitHub%20Training%20-%20Basic.md)

#### Step 3: Setup Git
 - The commands below will configure Git. Be sure to enter your own information inside the quotes (but include the quotation marks)!
```
git config --global user.name "Your Name"
git config --global user.email "yourname@example.com"
```
#### Step 4: Adding Token to Git
- Open command prompt and run below:
```
(echo url=https://github.com & echo username=username & echo password=your_access_token) | git credential approve
 ```


## Local to GitHub 
```
(a) "git init foldername" or to create a repo in the folder you are in, use "git init"
(b) Create a file, add content, then use git add and commit.
(c) Create a repository with the folder name on GitHub. Copy the repo link.
(d) In the VS terminal, type "git remote add origin 'http...'"
(e) When you try to push, it shows an "Error" because the remote GitHub repo already has an "initial commit" with a README.md, which was auto-created. Therefore, use the following steps:
  git pull
  git push origin main
```

## GitHub to Local 
```
(a) Create a repo on GitHub, then copy the link.
(b) In the VS terminal, use "git clone http..."
(c) git add, commit, push
```

## Creating branches with:
 - git branch <branch_name> or 
 - git checkout -b <branch_name> 

## Merging
 -  #### Note ensuring we are in the main branch:
     - git checkout main
     - git merge feature1 -m "merging feature1 back to main"


## Git Visualization 🖼️
![Alt Text](assests/Git%20visualization.png)


## Personal Access Token 🖼️
![Alt Text](assests/Personal%20Access%20Token%20SS.png)

## Pull Request 
1. Setting Branch Protection Rules
    - Go to your repository Settings.
    - Navigate to Branches.
    - Set protection rules for the desired branches.
    - Choose the first branch name pattern.

![Alt Text](assests/Pull%20Req%201.png)

2. Merging Process
    - Review and approve the changes.
    - Merge the branch into the main branch.

![Alt Text](assests/Pull%20Req%202.png)


# Folder Structure 📂 


```
GIT TRAINING - AMAN SIR/         # Main folder
│
├── assets/                      # Folder for images & documents
│   ├── Git visualization.png
│   ├── GitHub Training - Basic.md
│   ├── GitHub Training - Branches.md
│   ├── GitHub Training - Pull Requests.md
│   ├── Personal Access Token SS.png
│   ├── Pull Req 1.png
│   └── Pull Req 2.png
│
├── git-merge-test/              # Folder for merge testing
│   └── merge.txt
│
├── PPT/                         # Folder for presentations
│   └── Branching Philosophy.pptx
│
├── testing-inventyv/            # Testing-related tasks
│   ├── hello_world.txt
│   └── README.md
│
├── website-flow/                # Website-related files
│   ├── hotfix.txt
│   ├── index.html
│   ├── new_edition.html
│   ├── style.css
│   
│
└── README.md                    # Main documentation
```
