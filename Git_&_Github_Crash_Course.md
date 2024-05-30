1. Download and install Git on your system: https://git-scm.com/download

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

3. When you have some new code repo on your local system , so as a first step you should open a terminal and set the location to the repo's folder and then hit

   ```
   git int # this will intiallize the project in git by creating invisble .git folder
   ```

4. Stagging files and creating commits
