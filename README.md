## Case 1 - Push exisiting repo
* Create local directory with files and sub directories
* Create a local repo and some comits
* Create a repo on github 
* Copy the URL
* Back in VS Code open a console
* Type in : git remote add origin https://github.com/...
* Then : git remote show origin
* Fianlly : git push -u origin master

## Case 2 - Clone a repo
* Create a repo on github 
* Copy the url : https://github.com/40tude/TestVSCodeGitHub.git
* Open VS Code
* F1 then type **Git** in the bar, then select **Git : Clone**
* Copy the url
* Indicate where the repository should be cloned locally on the hard disk
	* Note : a subdirectory with the name of the cloned repo will be created beneath the selected directory
* Answer **yes** when VS Code ask to open the cloned repository
* For example, create and edit one file in the workspace
* Save the file
* The git icon should show the number of files impacted (1 here)
* CTRL+SHIFT+G to activate the Git panel in the left bar 
* Enter a message then press Ctrl + ENTER
* The file is now commited locally
* Click on the "..." and select **Push**
* You may have to type you're Git credentials
	* If you get tired read "About entering credentials" below
* You're done!



## Branching
* Open main.cpp
* Click on "master" in the bottom left
* Give a name to the branch (name it "branch" for example)
* Add a line to main.cpp (getchar(); on line 5 for example)
```cpp
getchar(); 
````
* Save the main.cpp file
* CTRL+SHIFT+G
* Enter a sentence ("Add getchar" for example)
* Press CTRL+ENTER
* Click on "branch" in the bottom left and switch to "master"
* Line 5 disapear !
* To take the modifications into account in master make sure "master" is visible in the bottom left corner
* Press F1
* Type "git mer..."
* Select "git merge option"
* Select the branch you want to merge ("branch" in our case)
* The main.cpp now have a getchar() finction call on line 5
* We can now delete "branch"
* F1
* Type "git del..."
* Select "git delete branch"
* Select the branch you want to merge ("branch" in our case)
* Make a push on github (see above the previous instructions)

## About entering credentials
In a terminal type : 
```bat
git config --global credential.helper wincred
```
You should then no longer be worried

Feel free to read : https://github.com/Microsoft/vscode/issues/26573


## YouTubegraphy
1. https://www.youtube.com/watch?v=6n1G45kpU2o
2. https://www.youtube.com/watch?v=9cMWR-EGFuY

