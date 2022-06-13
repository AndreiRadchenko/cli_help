### Arduino Help:
- Start arduino from folder arduino-1.8.10:

        andrei@E330 ~/arduino-1.8.10 $ ./arduino
        
- Enable acces to ttyUSB0:

        sudo chmod ugo+rw /dev/ttyUSB0
        
### Git help:
- Create remote repository:
- View pc ssh key for copy to github:

        cat ~/.ssh/id_rsa.pub

- Create a new repository on the command line

        echo "# WebMicGain" >> README.md
        git init
        git add README.md
        git commit -m "first commit"
        git remote add origin git@github.com:AndreiRadchenko/WebMicGain.git
        git push -u origin master
        
- Add remote repository:

        git remote add origin git@github.com:AndreiRadchenko/RF-Gate.git

- Add files and folders to local git:

        git add FreeRTOS/*
        git add readme.md
        git add uno-gate.sch

- View files under git:

        git ls-files

- Commit changes to current branch:

        git commit -a -m "change max load to 3A"

- Push commit to remote rep:

        git push -u origin master

- Create new branch and switch to this branch:

        git checkout -b current_sensors  

        git commit -a -m "change max load to 3A"
- View current changes from last commit:

        git diff
        git status

- Push new branch to remote repository:

        git push -u origin current_sensors

- Pull from remote repository:

        git pull
        git merge <branch>

- Show all branches:

        git branch -a

- Switch to branch <current_sensors>:

        git checkout current_sensors

- Revert to previos commit without saving changes:

        git reset --hard HEAD~1

- Revert to 2 commit with saving changes:

        git reset --soft HEAD~2

- Viewing the Commit History of branch <master>

        git log master
        git log --pretty=oneline
      
- First commit        
        
        git init
        git add .
        git commit -am "First commit"
        git remote add origin git@github.com:your_github_user/myapplication.git
        # Get the README and .gitignore files
        git pull origin master
        # Send the entire application to Github
        git push origin master
