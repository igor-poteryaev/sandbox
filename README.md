# sandbox
Experimental playground

Here I'll execute the ranming of the non-master branch to master for repository hosted on github.

Steps

1. Create the repository named 'sandbox' on github using my personal account. Done.
2. pull it to my local machine. Done.
3. Create a new branch named 'newmaster'. Done.
4. Make one new commit on it.
5. Switch back to master. Make one new commit there.
6. Push all local commits to github.
7. Change default github branch to 'newmaster'
8. Rename branch 'master' to 'legacy_master' both locally and on github  https://gist.github.com/lttlrck/9628955
9. Rename branch 'newmaster' to 'master' both locally and on github


commands 
# preparations

git branch newmaster
edit README.md
git add .
git commit -m "one commit on newmaster"
git co master
edit README.md
git add .
git commit -m "one commit on master"
git push
git co newmaster
git push

#
git branch -m master legacy_master
git push origin :master
git push --set-upstream origin legacy_master

#
git branch -m newmaster master
git push origin :newmaster
git push --set-upstream origin master
