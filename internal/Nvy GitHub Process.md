# Nvy.io GitHub Initialization Process

## [Personal Checklist]

## Create the GitHub Repository (Manual)

### Steps to Create A Repository Manually

From within Github:

1. Select `New Repository` [upper right corner]
1. Enter Repository Name and a Description
1. Choose Appropriate Options
    a. Public
    b. Add a readme
    c. Select gitignore
    d. Select License [match to npm]
1. Do not add a read me
1. Review setup

#### Note the Repository Url

This will be used later to link the respository and the project.
    -- Example ( https://github.com/NvyMax/nvy_widgets.git)

## Create the Link

### Supress Private Files and Folders

In VSC: 
    -- Create the .ignore folder
    -- Add any files needed to the .gitignore file or folder

#### Initialize the Repo [Terminal]

From the Terminal type:

```git
git init
 ```

#### Add Credentials

From the terminal, type the following:

-- use `git config --list` to view current configuration settings

** Add [as needed]: **
`- git config --global user.name "NiKole Maxwell"`

`- git config --global user.email "nvymaxwell@outlook.com"`

`git status` This will pull the current status, nothing should be committed yet

verification msg:  *"nothing added to commit but untracked files are present"*

### Link to Remote Repository [Terminal]

1. Type `git remote` , this starts the git remote listener
1. Type `git remote add origin +  https://github.com/NvyMax/NAME.git` Name = the name of your repo. 
    -- This should be the project url.
1. Type `git remote` again (git should report "origin")

### Add existing files to Git

1. Type `git status` to review adds and files being supressed
1. Type `git add .`  to add all files you want tracked to the staging area, if there are files that need to be added to .gitignore do so.
1. Type `git status` review the files being added and suppressed

### Commit files from the Staging Area to the Master

 1. Type `git commit -m` + " Message to be displayed on Github regarding the commit" example: "Initial commit: Create Repo"
   a. Alternatively you can type `git commit  "comment"`
   b. This can also be used to update tickets from the ISSUE tracker.
   -- **Example:**  *Type Closed + the ticket number to automatically update*

### Push Files to Master (Terminal Push to GitHub)

1. Type `git push -u origin master`
1. Update the readme if necessary

## Handling Changes

### To Process Changes to Origin

Small changes are commits.  (a package of changes, generally representing a patch (major or minor).

To update commits for this project, they will be tracked directly by Visual Studio Code(VSC). 
When ready to commit them:

1. Update/any files that don't need to be tracked, to the GH repo
1. Save all open files
1. Click the Github button on VSC
1. Look at the number of changes to confirm this is how you want to proceed
1. You can use the links on the GH tool to change tasks (like make changes, merge pull ect.
1. Press the `+` button to stage all changes
1. Push the Git checkmark to update all of the commits to GH.
1. Input a comment about the updates
1. Items will update in the Terminal and will be pushed to the repo.

For additional updates look at the file called "github_process.txt"

## Add or Update Versioning

### git tag -a [version] -m "[version message]

#### git tag -a v1.2.0 -m "Awesome Library v1.2.0"

## Change the Name of a Repository/Url

git remote set-url origin [:https://github.com/MaxNvy/Valley_Girl_Jane](https://github.com/MaxNvy/Valley_Girl_Jane.git)
