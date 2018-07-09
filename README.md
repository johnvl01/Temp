# Temp

#easily-keep-gh-pages-in-sync-with-master
 git checkout gh-pages // go to the gh-pages branch
$ git rebase master // bring gh-pages up to date with master
$ git push origin gh-pages // commit the changes
$ git checkout master // return to the master branch

Thanks for this code snippet!

Here is an alias to run after git push origin master. Place this in your .gitconfig, mine is located in ~/Users/danielstepanov/.gitconfig

[alias]
	sync-ghpages = !git checkout gh-pages && git rebase master && git push origin gh-pages && git checkout master
Once added, you can run git sync-ghpages and it will automatically do the second half of the above code. I'm extremely lazy.

