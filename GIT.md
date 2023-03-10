# First commit
1. Create git repository

```git
git init
```

2. Add all files to the repository

```git
git add .
```

3. Commit changes

```git
git commit -m "MESSAGES"
```

4. Connect the local repository to github

```git
git remote add origin git@github.com:hxyv/###.git
```

5. Pull online repoistory to local before first push

```git
git pull origin main
```

6. Push changes to github repository

```git
git push -u origin main
```

### Override any checks that git does by using "force push"
```git
git push -f origin main
```
