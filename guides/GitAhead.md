# GitAhead client

## Clone a repository
![Git clone URL](../img/gitahead/github_clone.png)

Under the Code menu you can clone the repository using the URL that is shown here in GitHub by clicking on the clone button

## Top menu
![Menu](https://cdn.discordapp.com/attachments/723876866523529276/724187878044860436/unknown.png)

This menu is a really important one. I'll explain most of the buttons here, the ones not explained are either not important or should speak for themselves.

### The Fetch button
![Fetch button](https://cdn.discordapp.com/attachments/723876866523529276/724189298030542868/unknown.png)

This button will fetch changes from GitHub, but not update the files on your local machine.

### The Pull button
![Pull button](https://cdn.discordapp.com/attachments/723876866523529276/724189796540350494/unknown.png)

This is actually a menu, but you probably won't need to use the items in the menu. Pulling does the same as fetching, but also updates the code on your local machine if there is newer code in GitHub.

### The Push button
![Push button](https://cdn.discordapp.com/attachments/723876866523529276/724190612382941215/unknown.png)

When you have committed your files and are ready to push it to GitHub you can push this button. It'll show a number depending on how many commits you are pushing.

![Push error](https://cdn.discordapp.com/attachments/723876866523529276/724207475464863744/unknown.png)

When pushing you may encounter this error, click on "push and set the current branch's upstream" and it should get pushed now.

### The Checkout button
![Checkout button](https://cdn.discordapp.com/attachments/723876866523529276/724194180683006022/unknown.png)

If you want to switch to another branch, you can use this button.

### The Stash buttons
![Stash and Pop Stash button](https://cdn.discordapp.com/attachments/723876866523529276/724196236206538803/unknown.png "Stash | Pop Stash")

You may encounter a moment where you can't pull from GitHub due to a so called "Merge Conflict". In that case you can use the Stash and Pop Stash function if you want to keep your changes. First you Stash your changes by clicking on the left button, after that you pull from GitHub and you can use the Pop Stash button to reapply your changes to the files.

## How to create a new branch
![Creating a new branch](https://cdn.discordapp.com/attachments/722434771422019584/723874342957613137/unknown.png)

First open the branch menu and press New Branch.


![Name the branch](https://cdn.discordapp.com/attachments/723876866523529276/723876877483114597/unknown.png)

Follow the naming scheme of `username-change_name`, so for example: `goldelysium-contribution_guide`. Also make sure to have "Checkout branch" ticked so that you automatically change to it. Most of the time you want to have master as start point.

## Creating commits
![](../img/gitahead/commit_message.png "Commit message")

If you made changes to files, it'll show "Uncommittted changes" in the git timeline. Write a commit message with a title on the first line, skip a line and then you can put a detailed message if needed. Sometimes only a title is enough.

Click on stage all if you want to commit all the files you've changed, otherwise select the files or even the lines that you want to commit. After you've done that you can commit and push it.
