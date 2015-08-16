# Git With Teams

This document was originally created for the General Assembly course [Intro to Agile Web Development] (https://generalassemb.ly/education/intro-to-agile-web-development/boston/15770).

## Table of Contents


## Setting Up Git & Github

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
ssh-add ~/.ssh/id_rsa
```

### Associate your key with Github

Copy your **public** ssh key to your clipboard.

```
pbcopy < ~/.ssh/your-ssh-key-name.pub
# the same ssh key name as you used above
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

> As seen on [Github](https://help.github.com/articles/generating-ssh-keys/)
