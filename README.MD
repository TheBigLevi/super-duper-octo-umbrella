## Research Report
# Research at least three(3) VCS

GITHUB
GITLAB
GITBUCKET

# Select a preferred VCS

GITHUB

# Identify pre installation requirements for the selected VCS

The pre installation requirements if you want to use the github is a github account.

# Identify installation procedures for VCS

To install the github CLI first run the following:
```
apt install git
```
Once installed the user will want to configure their the username that will be tied to their accounts whenever they make a commit, change, merge, push etc.

This can be done by runinng the following:
```
git config --global  user.name "<insert full name here>"
```
This will change their name for all repos from the current machine, if they wish to do it for the current working repository one would remove the global flag.

The same must be done for the users email.
```
git config --global user.email "<insert email here>"
```

Once configured the user will want to generate a SSH key so that they are able to pull repositories and commit to them in a secure manner.

To generate a SSH key run the following:
```
ssh-keygen -t ed25519 -C "your_email@example.com"
```
When promted to enter a file in which to save the key press enter.
Then when prompted for a secure passphrase, enter a secure passphrase.

Once generated you will want to copy you public ssh key to your clipboard, you can do this by:
```
pbcopy < ~/.ssh/id_rsa.pub
```

If pbcopy doesn't work, fin the hidden .ssh folder, open the file and copy it to your clipboard.

Once copied naviagte to your github account and click on your profile in the top right to get the drop down.
Then navigate to Settings > SSH and GPG keys, before clicking add new ssh key.

Paste in your public ssh key and give the title a meaningful name so that you know its this machine.
Then click add ssh key and follow the promts (if any) to confirm its you and add the key.

# Identify any installation disruptions to normal daily operations and communicate disruption via email to the appropriate person

To whom it may concern,

Under your directions I have successful conducted my report, and to my knowledge the only disruption that would occur in the implementation of the VCS is that of setting up the users accounts, and configuring them with their public SSH keys to ensure that our repositories are secure. 

The information provided in my report should be more than sufficient for staff to do this themselves and shouldn't take more than 15 to 30 minutes to complete the setup for all staff.

Yours sincerely,
Lachlan Read
