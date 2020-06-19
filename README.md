# Starting R

This is an RStudio.cloud project set up by StatPrep Annie to provide templates for other StatPREP instructors using R for their own courses. 

Many R packages are pre-installed in this project. These include:

- tidyverse
- mosaic (which automatically installs mosaicData, mosaicCore, and ggformula)
- mosaicModel
- learnr (which includes shiny, etc)
- knitr
- RCurl
- rsconnect

## Copying StatPrep Annie's StartUsingR project

1. Using your browser, login to your account on `rstudio.cloud`. The main page for your "workspace" will be displayed.
2. Open a new tab in the browser. Cut and paste exactly this URL into that new tab.
    `https://rstudio.cloud/project/40418`
    Annie's template will be copied into your workspace. It will open with a red "Temporary" in the top line.
3. Press "Save a permanent copy" so that you have your own, fully independent copy of Annie's StartUsingR project.

## Creating a GitHub repository for the StartUsingR project

Leaving your RStudio.cloud tab for a few moments, you're going to create a new repository on GitHub to use for publishing web pages from your project.

1. Login to GitHub. Once you have done this, access the +v dropdown menu in the upper right of the GitHub display:

    ![](images/new_repo1.png)
    
    Select "new repository"

2. In response to your selecting "new repository," GitHub will display a set-up page:

    ![](images/new_repo2.png)
    
    - Choose a suitable name for the repo. For instance, if this is to be a course site, you might use the name of the course, e.g. `Stat101`.
    - Once you have set the new repository's name, skip directly on down to the green "Create repository" button. Press it
    
3. GitHub will now display a "Quick setup page." Near the top will be a section that looks like this:

    ![](images/new_repo3.png)

Note the repo URL that appears in the editing box. It is composed from your GitHub user name and the name you selected for the repository. Keep that handy. Later, you're going to paste that URL into a command.


## Connecting your RStudio project to GitHub

Your task now is to connect your own copy of the StartUsingR project to GitHub. To do this, go back to your rstudio.cloud tab displaying your project.

1. In the Git tab in RStudio, select the "gear" menu and then "shell." 
    ![](images/new_repo4.png)

    This will open up a new tab called "Terminal", next to the console.

2. In the Terminal tab, cut and paste these commands, making sure to **provide your own email address and name** rather than StatPrep Annie's. (If you have multiple email addresses, or multiple names, you can use any of them!) 

```r
git config --global user.email "StatPrep.Annie@gmail.com"
git config --global user.name "StatPrep Annie"
```
    Press enter. There will be no response by the computer. You're going to be using the terminal tab later, as well.

3. Give the command, in the terminal tab, that will instruct RStudio to refer to your GitHub repository. The command will look like the following, but **you must** change `USERNAME` to be your own GitHub username, and change `REPOSITORY` to be your own repository, set up in Step (1) of this section.
```
git remote set-url origin <paste_your_repo_URL_here>
```
    Again, when you press "enter", the computer will not respond.

4. In RStudio, open up some file, say, `README.Rmd`, and make some trivial change, such as adding a space after the document title. Then save the file.

5. In RStudio, go to the Git tab. You will see the name of the file you just edited (and maybe some others). Check the little box under "Staged" to the left of the file name. Then, press Commit.

6. A new window will open that looks like a bigger version of the Git tab. 

    ![](images/new_repo6.png)

    Write some short message in the box and press the "commit" button underneath the message box. 

7. Finally ... Press the green upward pointing arrow above the message box. You will be prompted to enter your GitHub account ID and password. Do so.

