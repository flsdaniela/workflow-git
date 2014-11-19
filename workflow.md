
### Git Workflow 

#### Create a new repository

You want to create a new repository in your PC (local repository) and then connect it with Github. A good practice is to create first your local repository and then create a repository in Github. Another good practice is to name both repositories the same.

You may proceed as follows in your local directory (assuming you are in the root directory):

1. Make a directory (some-directory) within your root directory:
        
        `mdkir some-directory` 

2. Change to the new directory:
        
        `cd some-directory`

3. Declare the directory as an actual repository: 

        `git init` 

4. Once you have declared the directory as a repository, it may or may not have a file. You can manually copy a file or create it with the following command:

        `touch some-file`

5. Now you are ready to add the exant files to the repository in order to make your first commit:

        `git add --all` or `git add some-file`

6. You have added the files (or a set of files) and there are ready to be commited to the repository, so you may proceed as follows:

        `git commit -m "some-message"`

where some-message is a mandatory description of the commit. 

7. Once you have commited the files, you may want to create a repository in the Github and connect both repositories. Go to your Github account, Create new > New repository, give the *same* name as your local repository.

8. Once you have made your repository in the Github, you may want to connect your local repository with a repository in the Github. To do this, type the following commands:

        `git remote add origin https://...`

        `git push origin master`

The first code line connects your local repository with your repository in the Github (actually the url provided is the one you get in your specific repository website). The second code line just tells Git to upload to Github the files previously commited.






