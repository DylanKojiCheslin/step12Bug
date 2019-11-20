
# Vulcan Starter bug step 12

this is a reproduction of a  missing behavior bug in Vulcan-Starter  
on step 12 there is intended to be the "user's displayName next to their review"  
it is a two repo installation with both on "devel" branch at 1.14.0 


![Image of missing displayName](../devel/Screenshot%20from%202019-11-20%2006-42-22.png)

OS: Ubuntu 18.04.3 LTS

## bug reproduction steps

1 clone this repo  

2 create a settings.json file  

3 create dir and inside it clone Vulcan core repo and change it to the "devel" branch 1.14.0 or use existing core repo on "devel" branch 1.14.0  

4 run with following, but change it to point to your core vulcan repo  
```
METEOR_PACKAGE_DIRS="/home/dylan/Documents/http/vulcanBugRepos/1/Vulcan/packages" meteor --port 3000 --settings settings.json
```

5 install any necessary dependencies  

6 navigate to step 12 : relations page at http://localhost:3000/step/12  