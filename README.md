# Git Branching
Today we're going to learn how to write software as a team. One of the biggest obstacles software engineers face, is managing the contributions of a team of people, to a single project. Git allows us you to keep your changes separate from everybody else, until your work is complete. Lets see how this works.

## Create your first branch
Method 1:  
On the bottom left corner of your editor you should see the word `main`.  Click on `main` and a dropdown will open at the top of the screen. Select the `+ Create new branch...` option. Enter a name for your new branch and hit Enter.

Method 2:  
Press `ctrl+shift+p` to open a dropdown. In the dropdown search for `Git: Create Branch...` and select that option. Enter a name for your new branch and hit Enter.

You should notice now that `main` (bottom left corner of your editor) has been replaced with the name of your new branch. This simply indicates which branch you are on, first you were on `main` and now you are on your newly created branch. Lets see how branches work.

## Edit the file tic-tac-toe.txt
Open tic-tac-toe.txt. You'll notice it is O's turn. Go ahead and edit the file to play O's next turn. Save your changes.

## Review your changes
Go to the `Source Control` view. You can get there by clicking the 3rd icon from the top on the left side of the editor. You can also get there with `ctrl+shift+G`. This view will list all of the files you've changed, so you should see tic-tac-toe.txt there now. Click on the file to see the `diff`.

## Reading the diff
The `diff` shows the differences between the original version of the file and the current version of the file. Each changed line will be highlighted red or green. Green indicates an addition and red indicates a delete. The move you played for O should be highlighted in green.

## Commit your changes
Hover your mouse over `tic-tac-toe.txt` in the `Source Control` view. You should see a `+` icon to the right. Click that to `stage` your file. Now that your file is `staged` you can click the `Commit` button to `commit` your staged changes.

## Push your changes to remote
Everything you've done so far has changed only your local copy the files. We now need to `push` those changes, so other developers can access them. If you look again at the lower left corner of the editor you should now see some up and down arrows with numbers next to them. The down arrow tells you how many changes you need to `pull` in to get 'caught up' while the up arrow tells you how many changes you can  `push`. Click that now, to sync your changes with the remote repo.

## Create your Pull Request.
The last step in making your code available to other developers is to create a `Pull Request`.
- Head on over to the [Branch Lab repo](https://github.com/qbranch4327/branch-lab/pulls) and go to the `Pull Requests` tab.
- Click on the New pull request button.
- Leave the `base: main` button alone. The base branch is the one we are merging our code in to.
- Click the `compare: main` button and in the dropdown choose the branch you created earlier.
- Click `Create pull request` and optionally fill in the comment box. Click `Create pull request` again.

That's it! You've successfully used Git to create your own, isolated `change set`, and created a `Pull Request` to integrate your changes back into the main branch.