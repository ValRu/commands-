## git

`git push origin --delete $(git branch -r | grep feature | cut -c10-100)`
removes all feature branches from remote (origin)


## docker 
`docker inspect --format="{{.NetworkSettings.Networks.nat.IPAddress}}" containername `
returns ip of container 


### windows
`echo findstr %1 %2 %3 %4 %5 > %systemroot%\grep.cmd`  then you can use `netstat -a -b | grep svchost`

`Set-ItemProperty -Path "HKLM:\SYSTEM\CurrentControlSet\Control" -Name "ServicesPipeTimeout" -Value "60000"` increases strarting timeout for windows services


`gwmi win32_loggedonuser  | select Antecedent` returns the list with active users
