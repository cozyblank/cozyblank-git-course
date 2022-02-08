# Browsing History

1. Make another commit. Now you should have two commits in your repo. 
2. Show the changes in the last 2 commits.  
3. Show all commits made by yourself. Use the one-liner option. 
4. Show all commits with GUI in their message. 
5. Show all commits with changes to file1.txt. Include the number of lines added/removed.  
6. Compare the last two commits.  
7. Check out the commit before the last commit. Note the detached HEAD in the terminal. Check out the master branch. 
8. Show the author of every line in file1.txt.  
9. Create a tag (v1.0) for the last commit. Show the history using the one-liner option and note the tag you just created. 
10. Delete the tag.  

## Solutions
1. Make another commit. Now you should have two commits in your repo. 
```javascript
git add . 
git commit -m “Update file1” 
```
2. Show the changes in the last 2 commits.  
```javascript
git log --patch -2 
```
3. Show all commits made by yourself. Use the one-liner option. 
```javascript
git log --author=“Your name” --oneline 
```
4. Show all commits with GUI in their message. 
```javascript
git log --grep=“GUI” 
```
5. Show all commits with changes to file1.txt. Include the number of lines added/removed.  
```javascript
git log --stat file1.txt 
```
6. Compare the last two commits.  
```javascript
git diff HEAD~1 HEAD  
```
7. Check out the commit before the last commit. Note the detached HEAD in the terminal. Check out the master branch. 
```javascript
git checkout HEAD~1 
git checkout master
```
8. Show the author of every line in file1.txt.  
```javascript
git blame file1.txt 
```
9.  Create a tag (v1.0) for the last commit. Show the history using the one-liner option and note the tag you just created. 
```javascript
git tag v1.0 
git log --oneline 
```
10. Delete the tag.  
```javascript
git tag -d v1.0
```