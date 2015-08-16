# Git With Teams

This document was originally created for the General Assembly course [Intro to Agile Web Development] (https://generalassemb.ly/education/intro-to-agile-web-development/boston/15770).

## Table of Contents

- [Setting up Git with Github](#setting-up-git-with-github)
- [Starting a team project](#starting-a-team-project)

## Setting Up Git with Github

### Sign up for Github

Visit [github.com](http://github.com) and sign up. No surprises.

### Generate an ssh key on your terminal

Go to your `.ssh` folder

```
cd ~/.ssh
```

Generate a new ssh key

```
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
# Enter a name for your key, for example "personal-github"
# Enter a passcode (don't forget it!)
```

Ensure your ssh-agend is running

```
eval "$(ssh-agent -s)"
```

Add your key to the ssh-agent

```
ssh-add ~/.ssh/your-ssh-key-name
# eg. personal-github
```

### Associate your key with Github

Copy your **public** ssh key to your clipboard.

```
pbcopy < ~/.ssh/your-ssh-key-name.pub
# eg. pbcopy < ~/.ssh/personal-github.pub
```

Add the key to Github:

- Open Github
- In the top right corner of any page, click your profile photo, then click **Settings**.
- In the user settings sidebar, click **SSH keys**.
- Click **Add SSH key**.
- In the Title field, add a descriptive label for the new key. For example, if you're using a personal Mac, you might call this key "Personal MacBook Air".
- Paste your key into the "Key" field.
- Click **Add key**.
- Confirm the action by entering your GitHub password.

### Confirm everything Works

```
ssh -T git@github.com
```

## Starting a team project

### Pick a team lead (TL)

Select a person in your team to be the TL.

### Setup your new project

> Only the TL needs to do these steps.

1. Create a repository
  - Go to Github
  - Click the "+" button
  - Click **New repository**
  - Give the repository a name (eg. ga-git-with-teams)
  - Select **Public**
  - Check **Initialize this repository with a README**
  - Click **Create repository**
1. Grant access to the team members
  - Open the repository page
  - Click **Settings**
  - Click **Collaborators**
  - Add your team mates by email or Github account

### Clone the repo to your machine

> All team members should do these steps.

1. Go to the repo page
1. Under "You can clone with  HTTPS, SSH, or Subversion." click **SSH**
1. Copy the ssh url (eg. `git@github.com:gbanis/ga-git-with-teams.git`)
1. Open your terminal and navigate to your code folder
  - `cd ~/code`
  - or if you don't have one `mkdir ~/code && cd ~/code`
1. Clone the repo to your machine
  - eg. `git clone git@github.com:gbanis/ga-git-with-teams.git`
1. Navigate to your repo's folder
  - eg. `cd ga-git-with-teams`




