# Git

## How to print pretty git log

### type1
```
git config --global alias.logs "log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --date=relative"
```

### type2
```
git config --global alias.lg "log --color --graph --pretty=format:'%C(#dc322f)%h%C(#b58900)%d %C(#eee8d5)%s %C(#dc322f)| %C(#586f75)%cr %C(#dc322f)| %C(#586e75)%an%Creset' --abbrev-commit"
```

# remove specific file from git cache
```
git rm --cached filename
```

# remove all files from git cache
```
git rm -r --cached .
git add .
git commit -m ".gitignore is now working"
```
