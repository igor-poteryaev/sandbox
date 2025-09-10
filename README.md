# sandbox
Experimental playground

Here I'll execute the renaming of the non-main branch to main for repository hosted on github.

Steps

1. Create the repository named 'sandbox' on github using my personal account. Done.
2. pull it to my local machine. Done.
3. Create a new branch named 'newmain'. Done.
4. Make one new commit on it.
5. Switch back to main. Make one new commit there.
6. Push all local commits to github.
7. Change default github branch to 'newmain'
8. Rename branch 'main' to 'legacy_main' both locally and on github  https://gist.github.com/lttlrck/9628955
9. Rename branch 'newmain' to 'main' both locally and on github


commands 
# preparations

```
git branch newmain
edit README.md
git add .
git commit -m "one commit on newmain"
git co main
edit README.md
git add .
git commit -m "one commit on main"
git push
git co newmain
git push
```

#
```
git branch -m main legacy_main
git push origin :main
git co legacy_main
git push --set-upstream origin legacy_main
```

#
```
git branch -m newmain main
git push origin :newmain
git co main
git push --set-upstream origin main
```
