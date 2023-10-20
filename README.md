# Git-Github
Initializing Git For Version Control

Setting up Git for the first time on a new project is fairly simple, you just need to enter these five commands into your terminal. Be sure to be sitting in the directory where your project is located!

You only need to do this once, right when you start your new project. If you create a completely new project, you’ll have to go through these commands again. But only once per project…



$ git config --global user.name "Your Name"

$ git config --global user.email "you@youraddress.com"

$ git config --global push.default matching

$ git config --global alias.co checkout

$ git init


<h1>Pull Requests</h1>

## Getting Started 🤩🤗:

- Fork this repo (button on top)
- Clone on your local machine

```terminal
git clone https://github.com/ossamamehmood/Hacktoberfest2023.git
```
- Navigate to project directory.
```terminal
cd Hacktoberfest2023
```

- Create a new Branch

```markdown
git checkout -b my-new-branch
```
- Make your changes `folderName/fileName`

- Add your changes
```markdown
git add .
```
- Commit your changes.

```markdown
git commit -m "Relevant message"
```
- Then push 
```markdown
git push origin my-new-branch
```


- Create a new pull request from your forked repository

<br>

## Avoid Conflicts {Syncing your fork}

An easy way to avoid conflicts is to add an 'upstream' for your git repo, as other PR's may be merged while you're working on your branch/fork.   

```terminal
git remote add upstream https://github.com/ossamamehmood/Hacktoberfest2023
```

You can verify that the new remote has been added by typing
```terminal
git remote -v
```

To pull any new changes from your parent repo simply run
```terminal
git merge upstream/main
```

This will give you any eventual conflicts and allow you to easily solve them in your repo. It's a good idea to use it frequently in between your own commits to make sure that your repo is up to date with its parent.
