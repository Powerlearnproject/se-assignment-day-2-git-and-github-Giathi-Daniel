# Question 1
 **Fundamental Concepts**
 - Individual changes to the code are represented as commits.
 - Branches enable parallel development allowing one to isolate specific features from the codebase, facilitating concurrent development.
 - Merging intergrates changes from different branches, combining them into the main codebase.
 - There are 2 main types of repositories:
    - Local repository -> directory that is on your own machine where you write and commit code.
    - Remote repository -> directory that is hosted on a server
 - Diffs highlight the differences between various versions of files, allowing you to see precisely any changes made between the commits

 **Why Github is a popular tool**
 - It alllows GIT intergration hence efficient in handling large projects.
 - It provides a robust system for code review and collaboration.
 - GitHub offers CI/CD features which allows one to automate workflows,run tests, and deploy code
 - It is an open source system, making it easier to contribute and collaborate on open-source projects

 **How Version Control Helps Maintain System Integrity**
 - Keeps history of changes, making it easier to understand the evolution of codebase
 - With version control, you have backup of your code and can recover your code if something goes wrong
 - It allows team work collaboration.
 - Version control system allows one to resolve conflicts betweeen multiple changes overlap, ensuring the final code is consistent and functional

# Question 2
**Setting up a new repo on GitHub**
- Create a GitHUb account
- Create a new repository; choose a unique name for your repo, provide a brief description of what the repo is for.
- Choose visbility; (public, private) according to your preference
- Add a README file for your repo, add .gitignore to exclude files tha should not be tracked
- Click Create repository button

**Important decisions to make**
- Repo Name and Description -> The name should be clear and descriptive, and the description should clearly explain the repo's purpose
- Visibility -> Choose between public and private based on the project's sensitivity and intended audience

# Question 3
- The README should start with the project's name and a concise description of its objectives and functionalities.
- For larger projects include a Table Of Content for easier navigation
- Ensure a detailed step-by-step guide for setting up the project locally
- The README should also include a contributing guidelines, outlining how others can contribute to the project
- License Info -> specifying the license under which the project is distributed
- Acknowledgements section for individuals, libraries, or tools that contributed to the project

# Question 4
**Differences betweena public repo and a private repo**
- Public Repositories
    - They are accessible to anyone on the internet hence fostering collaboration leading to richer quality code and more innovative solutions.
    - Some of the disadvantages of the public repositories is that; there is a greate rist of unauthorized changes or malicious contributionss. Furthermore, sensitive information can be exposed if not careful managed
- Private Repositories
    - Private repos restrict access to only those individuals or teams explicitly granted permission. The primary advantege is that, the owner have a complete control over who caan viewand modify the code.
    - On the downside, private repos can limit the scope of collaboration compared to public repos, limiting feedback from a broader audience.

# Question 5
**Steps to make yout first commit**
- Install Git and Create a GitHub Account
- Login to GitHub and Create a repo
- Obtain the repository URL and clone the github repository [`git clone URL`]
- Navigate to your repository directory and add files locally
- Add files to the staging area [`git add . `OR `git add file-name`]
- Record the staged changes with a commit message to describe what you've done. [`git commit -m "first commit message"`]
- Push the changes made to the remote repository on GitHub [`git push origin main`]

# Question 6
- Branching helps in managing development workflows, especially in colllabotatively environments. It allows developers to work on different features, fix bugs withouf interfering with the codebase.
- A seperate environment is created where changes can be done withouft affecting the main code.

*Importance*
-  Developers can work on changes independently without affecting the codebase
- It allows multiple features to be developed in parallel.
- Branching facilitates code reviews and testing before merging chages into the main branch

*Creating a branch*
- Check currenct branch [`git branch`]
- Create a new branch [`git branch footer`]
- Switch to the new branch [`git checkout footer`]
- Make changes to the branch, stage and commit the changes [`git add .`], [`git commit -m "Add footer"`]
- Push the branch to the remote repository [`gut push origin footer`]
- Switch to the target branch, pull latest changes and merge the footer branch to into the target branch
[`git checkout main`], [`git pull origin main`], [`git merge footer`]
- After merging, you can delete the branch locally
[`git branch -d footer`]

# Question 7 
**Pull Request**
- PRs provide ways for teams to review and discuss chanfes made before being marged into the main codebase, hence fostering collaboation to a project
- PRs seves as a record of chanfes, providing context and rationale behind modifications

*Steps in creating and merging a pull request*
- Create and make changes to a branch [`git ceckout -b navigation`]
- Once satisfied with your changes, stage and commit them [`git add .`], [`git commit -m "Create navigation"`]
- Push your branch to the remote repo on GitHub [`git push origin navigation`]
- Go to the GitHub repository and create a pull request; select your branch and the branch you want to merge, givign the title and description of the pull request
- Team members will receive the pull request, check out the changes made, suggest changes or give feedback to the pull request
- Make any necessary changes based on the feedback given from the review.
- Once the review has been addressed, the pull request in now approved and merged.
- After merging, delete the branch both locally and remotely [`git branch -d navigation`], [`git push origin --delete navigation`]

# Question 8
- Forking allows you to create a personal copy of a repository on your own GitHub account

*Forking*
- Creates a new repository on your GitHub account, that is a copy of the original repository
- It is essential when you want to contribute to an open-source project, you don't have write access to.
-  Forking allows you to customize the project according to  your preferences.
- Forking also offers an environment where you can learn and experiment with code in a practical settin

*Cloning*
- Cloning creates a copy of a repository on your machine locally.
- It allows you to make work on a project you have access to

# Question 9
*Importance of Issues*
- Issues document and tack bugs, including details and severity
- Manages tasks and break down larger features into smaller issues
- Also help in centralized communication about a specific issues

*Importance of Project Boards*
- Project boards visualize workflows, organize taks, and helps in tracking milestones.
- Support collaboration and accountability -> One can assign issues, track ownership, and ensure accountability

*Examples*
- Provides visibility into tasks and status, aligning team efforts
- Allows continuous communication on issues, suppporting iterative development and responsive improvements.
- Boards help prioritize taks and set deadlines, aiding in effective planning.

# Question 10
*Common challenges and pitfalls for using GitHub for version control*
- Newbies may struggle with understanding Git concepts such as branching, merging etc.
- Managing multiple branchs can be confusing in merging and resolving conflicts
- When merging occurs, different branches may overlap, creating difficulties in intergrating code.
- Inconsistency in commit messages, make it hard to understand the change being done
- Improper management of repositories permissions can lead to unauthorized access or accidentally leaking data

*Best Practices*
- Use a well-defined workflow, to manage branches and releases e.g Git Flow
- Implemeneting CI/CD piplenines can be effective to automate testing and deployment
- Document processes and convetions for easy preference for new contributors, and also maintain consistency
- Organize taks and track progress using GitHub Project Boards
- Regularly back up important repos in case of data loss or corruption issues