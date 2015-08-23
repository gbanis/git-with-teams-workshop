Create a file with your name and some favorite picks.

Instructions:

**Work on your changes**

- Create a branch
  - `$ git branch -d favorite-picks`
- Create a new empty file
  - `$ touch favorite-picks.md`
- Commit your changes
  - `$ git add favorite-picks.md`
  - `$ git commit -m "Created empty file favorite-picks.md"
- Copy and paste in the following template

    ```
    Name:
    Favorite food:
    Favorite animal:
    Favorite tv show:
    ```
- Commit your changes
  - `$ git add favorite-picks.md`
  - `$ git commit -m "Added the empty template"`
- Fill in your info
- Commit your changes
  - `$ git add favorite-picks.md`
  - `$ git commit -m "Added my info"`
- Push your changes to Github
  - `$ git push`
  - `$ git push --set-upstream origin favorite-picks`

**Review and merge your changes**

- Open Github
- Go to your repo
- Click `Compare & pull request`
- Click `Create pull request`
- Review your pull request
  - Look at `Files changed`
- Merge your pull request
  - Go to `Conversation`
  - Click `Merge pull request`
  - Click `Confirm merge`
  - Click `Delete branch`
- Update your local environment
  - Checkout master `$ git checkout master`
  - Update master `$ git pull`
  - Delete the feature branch `$git branch -d favorite-picks`



