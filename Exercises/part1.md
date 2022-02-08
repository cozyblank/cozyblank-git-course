# Creating Snapshots

1. Initialize a new repository. Add two files in your working directory.  
2. View the status of the working directory and the staging area. 
3. Stage both files.  
4. View the changes in the staging area.  
5. Create a commit.  
6. View the list of commits.  
7. View the content of the last commit.  
8. Update one of the files. View the changes in the working directory. 
9. Stage the changes.  
10. Unstage the file.  

## Solutions
1.  Initialize a new repository. Add two text files in your working directory.  
```javascript
git init  
echo hello > file1.txt 
echo hello > file2.txt 
```
2.  View the status of the working directory and the staging area.  git status  
```javascript
git status 
git status -s
```

3. Stage both files. 
```javascript
git add .
```

4. View the changes in the staging area.  
```javascript
git diff --staged 
```

5. Create a commit.  
```javascript
git commit -m “Initial commit.” 
```   

6. View the list of commits.   
```javascript
git log
```      

7. View the content of the last commit.   
```javascript
git show HEAD 
```   

8. Update one of the files. View the changes in the working directory.   
```javascript
echo world >> file1.txt git diff
```   

9. Stage the changes. 
```javascript
git add file1.txt
```   

10. Unstage the file.
```javascript
git restore --staged file.txt
```
