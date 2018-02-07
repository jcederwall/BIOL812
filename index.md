# BIOL 812 - Assignment 

## Jeffrey Cederwall



### Questions

#### 1. When should you use Git for a project?

Git should be used when you want to store and share all versions of a project. This can be helpful to have earlier versions of a project in case an error is made so you can refer back to a previous version. By having git accessible you can easily share your work with others to collaborate on projects. 

#### 2. What kind of files/info should be saved in a Git repository? What types of files/info should not be included in a Git repo?

Scripts, code, and test files should be stored in git repositories. It is not recommended to store sensitive information or large datasets in a git repository. 

#### 3. What are the commands to undo a commit?

To undo a bad commit, you can follow the following code below to reset to an earlier version and then change the file to what you want. This answer was found from [Stackoverflow][1].

[1]: https://stackoverflow.com/questions/927358/how-to-undo-the-most-recent-commits-in-git 
 
```
git commit -m "Something terribly misguided"              
git reset HEAD~  
```
<< edit files as necessary >>   
```
$ git add ...                                               
$ git commit -c ORIG_HEAD   
```

#### 4. One of your repositories is in a “detached HEAD” state. How do you fix this?

```
git checkout master
```

#### 5. Your boss has no idea what Git is or why you are using it. Explain the pros / cons of using Git for your research project. Explain the pros / cons of hosting your project in a public (or private) repository on Github/Bitbucket/Gitlab/etc.

##### Pros 
+ Allows you easily share information and code with collaborators 
+ Free to use
+ Will save earlier versions of your work in case of errors 
+ Can be used as back-up location for your R scripts in case of a computer error

##### Cons 
+ Publically accessible so it is not advised for sensitive information 
+ Private repositories are available but cost money  
+ Can be difficult to learn initially
