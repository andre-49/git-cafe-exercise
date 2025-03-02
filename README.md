# git-cafe-exercise

# BUNDLE 5

## EXERCISE 1
```
done
```

## EXERCISE 2

```
╭─andre@beBop ~/Cyphers/git_basics  ‹main› 
╰─➤  cd ../clones    
╭─andre@beBop ~/Cyphers/clones  
╰─➤  git clone git@github.com:andre-49/git-cafe-exercise.git
Cloning into 'git-cafe-exercise'...
remote: Enumerating objects: 107, done.
remote: Counting objects: 100% (15/15), done.
remote: Compressing objects: 100% (11/11), done.
remote: Total 107 (delta 5), reused 4 (delta 4), pack-reused 92 (from 1)
Receiving objects: 100% (107/107), 1.95 MiB | 54.00 KiB/s, done.
Resolving deltas: 100% (5/5), done.
╭─andre@beBop ~/Cyphers/clones  
╰─➤  cd git-cafe-exercise 
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹main› 
╰─➤  v index.html 
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹main*› 
╰─➤  git commit -am "changed index file"                    
[main 52c8c49] changed index file
 1 file changed, 2 insertions(+), 2 deletions(-)
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹main› 
╰─➤  git remote                         
origin
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹main› 
╰─➤  git push       
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 319 bytes | 319.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To github.com:andre-49/git-cafe-exercise.git
   d1d3f9c..52c8c49  main -> main
```

# BUNDLE 6

## EXERCISE 1

```
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹main› 
╰─➤  git checkout -b ft/menu            
Switched to a new branch 'ft/menu'
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹ft/menu› 
╰─➤  v menu.html                 
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹ft/menu*› 
╰─➤  git add .              
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹ft/menu*› 
╰─➤  git commit -m "menu page"               
[ft/menu 122f557] menu page
 1 file changed, 12 insertions(+)
 create mode 100644 menu.html
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹ft/menu› 
╰─➤  git push -u origin ft/menu     
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 443 bytes | 443.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/menu' on GitHub by visiting:
remote:      https://github.com/andre-49/git-cafe-exercise/pull/new/ft/menu
remote: 
To github.com:andre-49/git-cafe-exercise.git
 * [new branch]      ft/menu -> ft/menu
branch 'ft/menu' set up to track 'origin/ft/menu'.
```

## EXERCISE 2 & 3

```
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹main› 
╰─➤  git checkout -b bug-fix  
Switched to a new branch 'bug-fix'
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹bug-fix› 
╰─➤  mv index-4.html Contact
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹bug-fix*› 
╰─➤  git push origin bug-fix   
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'bug-fix' on GitHub by visiting:
remote:      https://github.com/andre-49/git-cafe-exercise/pull/new/bug-fix
remote: 
To github.com:andre-49/git-cafe-exercise.git
 * [new branch]      bug-fix -> bug-fix
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹bug-fix*› 
╰─➤  git commit -am "changed index-4.html to Contact"
[bug-fix 07244cf] changed index-4.html to Contact
 1 file changed, 204 deletions(-)
 delete mode 100644 index-4.html
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹bug-fix*› 
╰─➤  git push origin bug-fix                         
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 238 bytes | 238.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:andre-49/git-cafe-exercise.git
   52c8c49..07244cf  bug-fix -> bug-fix
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹bug-fix*› 
╰─➤  git status             
On branch bug-fix
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	Contact

nothing added to commit but untracked files present (use "git add" to track)
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹bug-fix*› 
╰─➤  git add . 
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹bug-fix*› 
╰─➤  git commit -m "changed index-4.html to Contact" 
[bug-fix 97cc6cb] changed index-4.html to Contact
 1 file changed, 204 insertions(+)
 create mode 100644 Contact
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹bug-fix› 
╰─➤  git push origin bug-fix                        
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 2.49 KiB | 2.49 MiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:andre-49/git-cafe-exercise.git
   07244cf..97cc6cb  bug-fix -> bug-fix
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹bug-fix› 
╰─➤  git switch main                                
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹main› 
╰─➤  v index-4.html 
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹main*› 
╰─➤  git commit -am "changed hot-fix telephone number"
[main abcebe4] changed hot-fix telephone number
 1 file changed, 2 insertions(+), 2 deletions(-)
╭─andre@beBop ~/Cyphers/clones/git-cafe-exercise  ‹main› 
╰─➤  git push                                         
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 310 bytes | 310.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To github.com:andre-49/git-cafe-exercise.git
   52c8c49..abcebe4  main -> main
```
