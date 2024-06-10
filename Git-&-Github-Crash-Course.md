1. Download and install Git on your system: https://git-scm.com/download

<br/>
<br/>

2. Configuring Git

After installing Git, you can also configure it - most importantly, you can set a username and email address that will be connected to all your code snapshots.

- This can be done via:
```
git config --global user.name "your-username"
git config --global user.email "your-email"
```
You can learn more about Git's configuration options here: https://git-scm.com/docs/git-config

Incase to check all the git global configurations, hit:
```
git config --list
```

And to know more about git commands or want to look into any specific git command, hit:
```
git help
```

<br/>
<br/>
<br/>
<br/>

<h1>Git Commands</h1>
<br/>
<br/>
<br/>
<br/>
3. When you have some new code repo on your local system , so as a first step you should open a terminal and set the location to the repo's folder and then hit

   ```
   git int # this will intiallize the project in git by creating invisble .git folder
   ```
   <img width="842" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/db6f3fb8-922d-4947-902e-0d960e6acf92">

<br/>
<br/>

4. Stagging files and creating commits
   <img width="1315" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/a7681c5d-ce70-4c59-bdeb-2c8431fe240a">

   - these commits are created so that you can anytime go back to any of these commits..
   -  from above image we learned
      - **git add <File(01) NAME> <File(02) NAME> <File(03) NAME>**: it will set the stage to commit
         - Another way to stage all files at ones is "**git add .**" or "git add *" . Downside of this approach is that it add all the files in the repo which may include any unwanted files..  and so you can add ".gitignore" file and mention files which you want git to ignore and Hence now you can use "git add ." and it will add only the required files and ignore the unwanted files(refere point # 9)
      - **git commit -m " ENTER YOUR MESSAGE HERE "**: it will commit the file(s) to git(not to github)
      - **git status**: it provide current status like is the file in stagging or commited, what all files etc..
      - **git log**: it will provide you all the commits you have done so far, with date-time and Unique ID of that commit...


<br/>
<br/>
5. Multiple Commits and Checking out Snapshots

<img width="1315" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/c19bccb6-8267-439f-be34-43d3f6fd96cf">
   
   - **git checkout <Commit ID # >** : it will change the "code" to the snapshot of that "commit id only" from the "latest code base". And if you check status (git status) "head" directs to the "commit id" which we provide. By default git "head" directs to latest "commmit id".
     
   - **git checkout main** : By anytime if you want to restore and go back to the latest head, just checkout to "main"(means "main branch") will restore everything. and now you will see the "code base" is again back to the previous latest state and you can check all the commits or status by "git status" where "head" will direct to the latest commit..

      **NOTE** - the git checkout is not delete anything, but it was tempraray change in commits..


<br/>
<br/>
6. Undo Commits or Reverting changes with "Git revert" 

<img width="1300" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/db1dca3b-e62d-45c5-ad1f-9905f159fb79">

   - From above image, if you have to revert the commint "C6", then by using "git revert < id-of-C6 >" this will create new commit as "C7" as shown form above figure. Note - its not deleting "C6", instead just creating new "C7".

   - **git revert <Commit ID # >** - it will revert the changes of commit by creating new commit (which is just absent of revert code). In one word it Undo commit



<br/>
<br/>
7. Removing commits or Resetting code with "git reset"

- **git reset --hard <Commit ID # >**  : to will delete all the commits which are before mentioned commit ID..
- For we have commits C1,C2,C3,C4,C5,C6 and now if you run "git reset --hard <C3 ID # >". It will delete C4, C5,C6 and we have following commits: C1, C2, C3 available only...


8. All the above Key commands in Git
   <img width="1251" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/6de5942b-a687-4bc1-9224-ac190fcfbeb7">



9. Stagging Multiple files and ignoring with .gitignore
    <img width="1114" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/b73fb92a-da40-4fad-b5ea-e369c84d27d8">

    - Create ".gitignore" file in your repository and include all the files names which you wanted to be ignored by git and not pushed, as shown in above image, which is ".vscode" and ".DS_Store"
    - now you can use "git add ." that this will stack all the files at ones and ignores all the files which are mentioned in the .gitignore file.
    


<br/>
<br/>
<br/>
<br/>

<h1>Branches</h1>
<br/>
<br/>
<br/>
<br/>


10. Understanding the Git Branches

   <img width="896" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/f2dcd4d8-3315-4b1f-955f-6324dfba7d1a">
   
   - When you intiatlize the git project with "git init", you get by default "main" branch(will contains all your commits)
   - **git branch < Name of Branch>** : it will create new branch, by default this will take your latest commit(as starting point) and create new branch, as shown above for "C2" commit for branch "feature-1" and then you can shift to new branch with **git checkout < Name of Branch** (eg git checkout feature-1)
   - **git checkout -b < Name of Branch>** : this is alternate way of creating new branch and started using it right away..
      - **git branch** : it will share all the exsisting branches names (with current branch name in green coloured and star)
      - **git branch -D < Name of Branch>** : it will delete the branch.
   - **git merge < Name of Branch>** : it will merge name mentioned in the command with the current active branch and automatically try to resolve the conflicts, for example as shown in above image we can merge "feature-1" to "main" branch. then acivate main branch by "git checkout main"(and check current branch by git log, main branch should be activate) and then merge "feature-1"  with main branch by git merge "feature-1" .. now after successful merged, this will show "how many files changed? how many lines added and delted"
     

<br/>
<br/>
<br/>
<br/>

<h1>Github</h1>
<br/>
<br/>
<br/>
<br/>


11. Github Intro
    <img width="1265" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/564561ea-6fe8-4a0c-ae4c-a2c965db0d82">


11. Connecting Local and Remote Repositories
   <img width="1222" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/62c9bd6c-3f2e-4e22-9625-5f95996b0c2b">

```
git remote add <Local repo Name> <github repo link>: #this will connect github to local git repository(eg git remote add origin https:github.com/abc/xyz.git)

```



12. pushing commit to github and understanding 
