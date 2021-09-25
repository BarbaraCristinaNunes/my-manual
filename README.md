# my-manual
## How to create a repository 

Open the terminal and discovery where you are! 

pwd => use this to discovery where you are 

ls => use this to see a list of folders 

In my case I am in /C/Users/barba (Home folder) 

cd ~ ==> use this to go to the Home folder 

cd ==> use this to go to the folder GitHub 

Now I create a folder which will be my new repository 

$ mkdir *folder name*

$ git init 

Now I have a new folder and the git sistem is booting 

So I am creating a README.md file 

$ touch *README.md*
After creating the README.md file, I gave it a git status and the file appears in red in the terminal. 

Files appear in red on the terminal because they have not been confirmed and have not yet been added (they are in Untracked status). This means that changes made to these files have not yet been saved. So I need to run git add and git commit to save these changes. After these steps, the file turns green on the terminal. 

(img\img1.png)

Now I have a repository with a file inside  

## Deleting a repository from the local environment 

$ rm –fr *folder name*

How to clone a repository  

When I want to clone a repository I go to GitHub, open my repository and select the Code button. In the Code button I select SSH and copy the link that is there. 

(img\img2.png)

Then I go to my terminal and write:  

$ git clone *copied link*

## How to create a local branch from the terminal  

In the terminal I need to be in my repository and type  

$ git checkout -b *branch name*

Sending the branch to the remote   

$ git push origin *branch name*

(img\img3.png)

(img\img4.png)

In this image I use $git status to see the files I changed.  

I did a $git add *filename* and a $git commit -m *"message"* to save the changes. 

 Then I gave a $git push to send to the remote repository   

## Doing MERGE   

I go to the main branch using $ git checkout *main*

So I give $git pull  

Then $ git merge *name of the branch I want to merge with main* 

 If there are no conflicts between the files I give a git push 

 ## Deleting a branch 

// delete branch locally git branch -d *localBranchName*

// delete branch remotely git push origin --delete *remoteBranchName*