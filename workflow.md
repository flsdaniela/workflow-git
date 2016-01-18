
### Git Workflow 

#### Create a new repository

You want to create a new repository in your PC (local repository) and then connect it with Github. A good practice is to create first your local repository and then create a repository in Github. Another good practice is to name both repositories the same.

You may proceed as follows in your local directory (assuming you are in the root directory):

* Make a directory (some-directory) within your root directory:
        
`mkdir <some-directory>` 

* Change to the new directory:
        
`cd <some-directory>`

Or probably you may want to copy an already existing repository in a remote server (usually the Github).

* Clone the remote repository to your local PC:

`git clone https://... <the url of the repo in Github>`


* Declare the directory as an actual repository: 

`git init` 

#### Changing files and adding to the staging area

* Once you have declared the directory as a repository, it may or may not have a file. You can manually copy a file or create it with the following command:

`touch <some-file>`

* If you modify this file, you need to add this to the staging area. This area contains all the changes you have made to your files. The command is as follows:

`git add --all` or `git add <some-file>`

#### Commiting the changes

* You have added the files (or a set of files) and there are ready to be commited to the repository, so you may proceed as follows (where some-message is a mandatory descrpition of the commit):

`git commit -m "<some-message>"`

* Once you have commited the files, you may want to create a repository in the Github and connect both repositories. Go to your Github account, Create new > New repository, give the **same** name as your local repository.

#### Pushing to the remote repository

* Once you have made your repository in the Github, you may want to connect your local repository with a repository in the Github. To do this, type the following commands:

`git remote add origin https://... <the url of the repo in Github>`

`git push origin master`

The first code line connects your local repository with your repository in the Github (actually the url provided is the one you get in your specific repository website). The second code line just tells Git to upload to Github the files previously commited.

By the way, you do not have to type `git remote add origin https://...` every time you push a file to your repo. This may be done only the first time you specify your directory as master. 

* If you are working on your local computer and want to update your local version with the latest version of a remote repository, you have to pull the changes down from the Github with:

`git pull origin master`

#### Viewing the differences

*Before you add your modified files to the staging area, you may want to view the differences: this can be done by typing the following command, which provides you an abbreviate and simple way to visualize the changes in your file:

`git diff --stat`

prueba
