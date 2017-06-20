## git

`git push origin --delete $(git branch -r | grep feature | cut -c10-100)`
removes all feature branches from remote (origin)

`git reflog -1 | sed 's/^.*: //'` shows a message of the last commit


## docker 
`docker inspect --format="{{.NetworkSettings.Networks.nat.IPAddress}}" containername `
returns ip of container 


## windows
`echo findstr %1 %2 %3 %4 %5 > %systemroot%\grep.cmd`  then you can use `netstat -a -b | grep svchost`

`Set-ItemProperty -Path "HKLM:\SYSTEM\CurrentControlSet\Control" -Name "ServicesPipeTimeout" -Value "60000"` increases strarting timeout for windows services

`gwmi win32_loggedonuser  | select Antecedent` returns the list with active users

`Get-EventLog -Newest 15 -LogName "Application"` gets latest events from EventViewer -> Windows Logs -> Application

`query user`  returns a list of logged on users

## kubernetes

`kubectl exec -it podsname  -- /bin/bash` starts the bash in specific pod

## grep

`grep -r 'AppFabric' . --include='*.config' | grep 'Live'` searches `AppFabric` word in all *.config files and then shows lines with `Live` word 

## sed
` sed -i 's/$OLD/new/g' filename.txt` updates all $OLD to "new" in the file
