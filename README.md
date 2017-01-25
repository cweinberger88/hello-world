# hello-world
Practice creating new repo

Already there's a different feel. I miss business school. I miss data analytics. This program I am in now and the data science immersive that I am trying to get in to, it's a challenge yes. It's something I can work towards, yes. But is the work really something I love? What about the environment? These are all factors I need to consider. 

How frustrating. 


[//]: # (charlie's comments below)
 
# charlie's comments
Hey there. I see you've made your repo public. That's great, because I can show you how pull requests and merges work. That's not so great because everyone can see the contents of this repo.

Here's what I did to clone your repo and start making commits:

1. Read the instructions here: http://kbroman.org/github_tutorial/pages/fork.html
   I followed these instructions exactly up until the step named "Add a connection to the original owner’s repository."
   
2. Modify your "README.md" file (the one you're looking at right now). I added these comments in notepad++. 

3. After I saved this file, I went back to the terminal and ran the following commands:

..1 `git status` - this shows files that are different from the local repository. In other words, after you've cloned a repo on your machine and modified+saved a file, it will show up in red here. 
    
	Here's the output from my machine after running this command:
```
$ git status
On branch master
Your branch is up-to-date with 'origin/master'.
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
```

..2 As you can see from the output above, I have made changes to the "README.md" file. I want to see what changed, so I run a "diff" command to see the *difference* between my working copy of the file and what's in my local repo. If you modify a file but don't add or commit, you will see those files here.

   Try running this on your own after you've modified a file:
   
   ```git diff README.md```
	
..3 Because I only changed one file, I will now do `git commit` (instead of `git add`). This is my personal preference. If you were editing multiple files, you could add them individually as you work on them, and once you have a working codebase, you `commit` all the changes at once. This way, you have one commit message for all the changes.
	
	```git commit README.md -m "committing my changes to README.md"
	
..4 Now that my changes are staged for push back to your repo, I will do the push:

    ```git push```
	
	If you would like to see a list of files you've staged for push, you can run the following command:
	
	``` git diff --stat --cached origin/master ```
	
	("origin" is the alias for the remote repository. In my case, this is your github "hello-world" repo.)
	("master" is the branch you want to compare against. If you are not on a branch, you are on "master".)

4. After step 3.3 above, I was not able to edit this document so I am writing this from the past. In the future, the right way to do this is for me to create a "branch" of your repository and push all my changes to that branch. When I am ready for you to look at my changes and merge them into the main branch, I would submit a pull request.
	
5. Next up: branches, merging, and more git fun.	
[//]: # (charlie's comments above)
