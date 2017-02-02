## git

`git push origin --delete $(git branch -r | grep feature | cut -c10-100)`
removes all feature branches from remote (origin)


##docker 
`docker inspect --format="{{.NetworkSettings.Networks.nat.IPAddress}}" containername `
returns ip of container 
