# Clone an existing repository
```
cd <<THE ROOT FOLDER FOR SOURCE CODE>>
mkdir <<A NAME TO REMEMBER WHAT THIS REPO IS>>
cd <<A NAME TO REMEMBER WHAT THIS REPO IS>>
git clone https://github.com/userAccount/project
```
----
# Create a new repository on command line
```
echo "# text for file" >> README.md
git init
git add README.md
git branch -M main
git remote add origin https://github.com/yourGitHubAccount/Hello-World.git
git push -u origin main
```
# Push an existing repository from command line
```
git remote add origin https://github.com/yourGitHubAccount/Hello-World.git
git branch -M main
git push -u origin main
```
####################################################################################################
#BEGIN:import code from another repository
####################################################################################################
import code
####################################################################################################
#*END*:import code from another repository
####################################################################################################
<CRLF>
<CRLF>
<CRLF>
<CRLF>
####################################################################################################
#BEGIN:Common Commands
####################################################################################################
#List all variables set in config file, along with their values.
git config --list

#configure git for your ident
git config --global user.email "_your_email@example.com_"
git config --global user.name "_yourName_"

#view git commit log
git log

#check status of project; displays changed files since last check
git status

#get difference since last commit
git diff

#check file changes since last commit
get status

#add files to commit
get add . 
get add myfile.ext

#create commit
git commit -m "[task#] initial commit"
####################################################################################################
#*END*:Common Commands
####################################################################################################
<CRLF>
<CRLF>
<CRLF>
<CRLF>
####################################################################################################
#BEGIN:install Git for Windows
####################################################################################################
#open command prompt and run the following command.
winget install --id Git.Git -e --source winget

####################################################################################################
#*END*:install Git for Windows
####################################################################################################
<CRLF>
<CRLF>
<CRLF>
<CRLF>
####################################################################################################
#BEGIN:setup ssh key
####################################################################################################
#open Git Bash
ssh-keygen -t rsa -b 4096 -C "_your_email@example.com_"
ssh-keygen -t ed25519 -C "_your_email@example.com_"

#check if ssh agent is enabled
eval "$(ssh-agent -s)"

#add ssh key to agent
ssh-add ~/.ssh/id_rsa

#cat public key to screen for copypasta to github
cat ~/.ssh/id_rsa.pub

#*add cat output to github
[https://github.com/settings/keys]
* Title: Meaningful title for this key. Technical Debt.
* Key: Past public key data here.
* {Add SSH KEY}

# Test github
ssh -T git@github.com
####################################################################################################
#*END*:setup ssh key
####################################################################################################