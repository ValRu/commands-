## git

`git push origin --delete $(git branch -r | grep feature | cut -c10-100)`
removes all feature branches from remote (origin)

