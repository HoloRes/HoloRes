# Contributing guide
**On the team? go to [here](#development-workflow), otherwise keep reading**

Welcome to the Hololive Resort Discord GitHub organization. This organization holds the code for some of our projects.

If you have suggestions for any repository: Feel free to create an issue

You want to contribute: Fork the repo, do your changes and feel free to create a PR (Pull Request).

Tips for when adding new features:

- Comment your code so others will be able to understand it
- Make sure in your PR you should give it a good title and list all the changes you made.
- For commits and PR's follow the [Git Commit Messages](#git-commit-messages) guidelines.

# Development workflow

## Table of contents

[Get started](#get-started)

[GitHub](#github)
- [Repository page](#the-initial-page)
- [Issues page](#issues-page)
- [Pull Requests page](#pull-requests-page)
- [Good to know](#good-to-know)

[GitAhead client](#gitahead-client)
- [How to clone a repository](#clone-a-repository)
- [The menu](#top-menu)
  - [Fetching](#the-fetch-button)
  - [Pulling](#the-pull-button)
  - [Pushing](#the-push-button)
  - [Checking out a branch](#the-checkout-button)
  - [Stashing](#the-stash-buttons)
- [Creating a new branch](#how-to-create-a-new-branch)

[Git Commit Messages guidelines](#git-commit-messages)

[The actual workflow](#the-workflow-itself)
- [Working on code](#working-on-code)
- [Reviewing someone's PR](#reviewing-someone-else's-code)

## Get started

First of all, download the [GitAhead client](https://gitahead.github.io/gitahead.com/) and login with your GitHub account. A lot of useful links are pinned in the Discord channel.

### Recommended software
These are only examples for if you don't already have stuff installed, all of the software listed is free or has a free version.

#### IDE:
- [Jetbrains IntelliJ IDEA](http://jetbrains.com/idea)
- [Visual Studio Code](https://code.visualstudio.com/)

#### Git clients:
- [GitAhead](https://gitahead.github.io/gitahead.com/)
- [GitKraken](https://www.gitkraken.com/)

#### Other software:
- [Node.js](https://nodejs.org/en): Since most projects are coded in JavaScript it's useful to have Node.js installed, make sure to choose the [**LTS(Long Term Support)**](https://nodejs.org/en/about/releases/) version. You can easily recognize LTS versions by checking if it's an even number.

### Useful sites
- [Google Fonts](https://fonts.google.com/)
- [Free for developers](https://free-for.dev/)

## GitHub

### The initial page
![GitHub repo page, with beta features enabled](https://cdn.discordapp.com/attachments/723876866523529276/723878776655577208/unknown.png)

When you open the GitHub repository, you'll likely see something similar to this.
Most of it should speak for itself but here a list anyway:

![Branch and tag viewer](https://cdn.discordapp.com/attachments/723876866523529276/723879530305159228/unknown.png)

The branches and tags viewer, this way you can look at the code of someone else is working on (in case of branches) or a specific version (in case of tags).

### Issues page
![Issues page](https://cdn.discordapp.com/attachments/723876866523529276/724006101485617222/xzEvCAuPnGwAAAAASUVORK5CYII.png)

This is the issues page, but it also has a few other purposes, here's a list:
- Feature requests
- Discussion
- Help requests for coding
- And of course bugs

Make sure to try to use the correct labels whenever you can. If you see an issue that hasn't been assigned to anyone yet, feel free to assign it to yourself if you can do it. Otherwise ask if you can help by commenting.

### Pull requests page
![Pull Requests page](https://cdn.discordapp.com/attachments/723876866523529276/724008999485440020/vFCdQnQIAAAQIECBAgQIAAAQIECBAgQIAAgeMCfpPkwokQIAAAQIECBAgQIAAAQIECBAgQIAAgesHLz08Ln88AsAAAAASUVORK5C.png)

The pull requests page is very similar to the issues page and the thing about labels is the same. Make sure it's a draft and optionally add `WIP:` in front of the title.

![Filter menu](https://cdn.discordapp.com/attachments/723876866523529276/724199942301941800/unknown.png)

You may notice something that is a bit weird. If you look at this you might think that I'm the reviewer for this PR, but that isn't the case.

![Hover over profile picture](https://cdn.discordapp.com/attachments/723876866523529276/724200348729737222/unknown.png)

If you hover over the profile picture, you will see I'm not the reviewer, but the person who this is assigned to. The bar above is to filter on users or status, but GitHub has made it a bit confusing.

## Good to know
- You can reference a Pull Request or Issue by using `#<ID>`, the ID can be found under the title on the overview page or next to the title on the issue page.
- In case you don't want to get spammed in your email from GitHub, you can disable the emails for specific notifications in your settings.
- GitHub has markdown, use it for longer issues or comments. Here is a [Cheat sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Here-Cheatsheet).
- Just as in Discord, you can ping users in a comment, issue or PR by using `@username`

## GitAhead client

### Clone a repository
![Git clone URL](https://cdn.discordapp.com/attachments/723876866523529276/723877829695242320/unknown.png)

Under the File menu you can clone the repository using the URL that is shown here in GitHub by clicking on the clone button

### Top menu
![Menu](https://cdn.discordapp.com/attachments/723876866523529276/724187878044860436/unknown.png)

This menu is a really important one. I'll explain most of the buttons here, the ones not explained are either not important or should speak for themselves.

#### The Fetch button
![Fetch button](https://cdn.discordapp.com/attachments/723876866523529276/724189298030542868/unknown.png)

This button will fetch changes from GitHub, but not update the files on your local machine.

#### The Pull button
![Pull button](https://cdn.discordapp.com/attachments/723876866523529276/724189796540350494/unknown.png)

This is actually a menu, but you probably won't need to use the items in the menu. Pulling does the same as fetching, but also updates the code on your local machine if there is newer code in GitHub.

#### The Push button
![Push button](https://cdn.discordapp.com/attachments/723876866523529276/724190612382941215/unknown.png)

When you have committed your files and are ready to push it to GitHub you can push this button. It'll show a number depending on how many commits you are pushing.

![Push error](https://cdn.discordapp.com/attachments/723876866523529276/724207475464863744/unknown.png)

When pushing you may encounter this error, click on "push and set the current branch's upstream" and it should get pushed now.

#### The Checkout button
![Checkout button](https://cdn.discordapp.com/attachments/723876866523529276/724194180683006022/unknown.png)

If you want to switch to another branch, you can use this button.

#### The Stash buttons
![Stash and Pop Stash button](https://cdn.discordapp.com/attachments/723876866523529276/724196236206538803/unknown.png "Stash | Pop Stash")

You may encounter a moment where you can't pull from GitHub due to a so called "Merge Conflict". In that case you can use the Stash and Pop Stash function if you want to keep your changes. First you Stash your changes by clicking on the left button, after that you pull from GitHub and you can use the Pop Stash button to reapply your changes to the files.

### How to create a new branch
![Creating a new branch](https://cdn.discordapp.com/attachments/722434771422019584/723874342957613137/unknown.png)

First open the branch menu and press New Branch.


![Name the branch](https://cdn.discordapp.com/attachments/723876866523529276/723876877483114597/unknown.png)

Follow the naming scheme of `username-change_name`, so for example: `goldelysium-contribution_guide`. Also make sure to have "Checkout branch" ticked so that you automatically change to it. Most of the time you want to have master as start point.

### Creating commits
![Commit message](https://cdn.discordapp.com/attachments/723876866523529276/724186386281791528/unknown.png)

If you made changes to files, it'll show "Uncommittted changes" in the git timeline. Write a commit message with a title on the first line, skip a line and then you can put a detailed message if needed. Sometimes only a title is enough.

Click on stage all if you want to commit all the files you've changed, otherwise select the files or even the lines that you want to commit. After you've done that you can commit and push it.

## Git Commit Messages

* Use the present tense ("Add feature" not "Added feature")
* Use the imperative mood ("Move cursor to..." not "Moves cursor to...")
* Limit the first line to 72 characters or less
* Reference issues and pull requests liberally after the first line

## The workflow itself

### Working on code
Now you know how the tools work, here is how it generally goes:
1. A feature is requested in Discord or in an issue
2. Let people know you're going to work on it by commenting in Discord or assigning in case of an issue.
3. Create a new branch
4. Start working on it
5. Commit and push
6. Create a PR, make sure to mark it as WIP if it isn't done yet and reference the issue if needed
7. When you're done, let **someone else** review it and merge it

### Reviewing someone else's code
**These are the things you want to look for:**
- Typo's
- Can you understand the code?
- Are the comments enough that you'll still understand it later on?
- Check for trailing whitespaces if possible
- If code is commented out, ask if it can be removed

**Some tips:**
- Select the correct review type
- Look at older PR reviews if you aren't sure if you're doing it correct
- Use multiline comments if it applies to multiple lines of code, you can do this by clicking on the `+` icon on the left side with the line numbers and drag it down until you selected all the lines you need.
-  Use Split mode instead of Unified, otherwise you may encounter issues with multiline comments

In case you still don't understand something, feel free to ask others on Discord. If deemed important enough, it will also get added into this guide.
