/*<!--this file should be able to guide on the initial installation for Git in the local system-->*/
First install Git in the computer and follow the installation process
For Windows there is direct installation file and for Mac go to <a href='https://brew.sh'> HomeBrew </a> and copy homebrew script in terminal then copy the required git script in terminal
once the installation is done then run the shell commands first try to link

<h2> For Windows</h2>>
1. First set the name or user name
Open Git Bash.

Set a Git username:

$ git config --global user.name "Mona Lisa"
Confirm that you have set the Git username correctly:

$ git config --global user.name
> Mona Lisa
2. Second after that setup email address
Open Git Bash.
Set an email address in Git. You can use your GitHub-provided no-reply email address or any email address.
$ git config --global user.email "email@example.com"
Confirm that you have set the email address correctly in Git:
$ git config --global user.email
email@example.com

<h2> For Mac </h2>>
Use Terminal instead of Git Bash rest follow same points 1. and 2. 

<h2> Linking local device with SSH on Git </h2>
Follow this <a href='https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent'> link </a> 

After connecting device with Github using SSH, we can either connect local repository to Github by linking it with <a href='https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository#adding-a-file-to-a-repository-using-the-command-line'> Github </a> or by creating a new one on Github and then using that one.
FYI for both the requirements we need to create a repository or project in Github by website I could not find a way directly to create a repo on Github by Git-Dash also it needs to be a new repo and not an existing one

After that to sync to Github
use command 
$ git remote add origin https://github.com/user/repo.git
$ git branch -M main
$ git push -u origin main
