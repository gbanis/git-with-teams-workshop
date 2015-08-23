# Creating and resolving a merge conflict

## STEP 1: Initialize your project

In this stage we will just create a basic skeleto to work with.

Only **one in each team** should to do this step.

- On `master`, create a new file
  - `$ touch boston-attractions.md`
- Open the file and paste the following:

  ```
  Favorite things to do:

  Favorite museums:

  Best restaurants:

  Best places to shop:

  Best bars:

  Favorite places to go for a walk:

  Best places to take photos:

  ```

- Commit changes and push
  - `$ git add boston-attractions.md`
  - `$ git commit -m "Basic template"`
  - `$ git push`
- Have your team pull the changes on their `master`
  - `$ git checkout master`
  - `$ git pull`

## Working together on a feature

Now all members will take an assignment and fill some of the fields.

Everyone will fill their `Favorite things to do`.

For the rest, self organize and pick the things you want to work on.

Name your branches based on the items you'll work on.

### Step 2 - Making your updates

**Team member 1**

- Branch off of `master`
  - `$ git checkout -b museums-restaurants`
- Make and commit your changes
  - `$ git add boston-attractions.md`
  - `$ git commit -m "Added museums and restaurants"
  - `$ git push` / `git push --set-upstream origin museums-restaurants`

Repeat for team members 2 & 3

### Step 3 - Merge with master

**Team member 1**

- Open a pull request on Github
- Ask for the other team members to review it
- Merge it

### Step 4 - Merge master and resolve conflicts

**Team member 2**

- If you haven't already, finish what you are working on and commit your changes
- Checkout `master` and pull the latest changes
  - `$ git checkout master`
  - `$ git pull`
- Checkout your branch and merge `master`
  - `$ git checkout shop-bars`
  - `$ git merge master`
- Let's resolve the conflicts!
  - Open your file and find the conflicts
  - Coordinate with your team-mates to decide what you need to keep
  - Commit your changes
    - `$ git add boston-attractions.md`
    - `$ git commit`

### Step 5

Repeat steps 4 and 5 for the rest team members.
