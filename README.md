## Steps
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
* The git icon should show the nunber of files impacted (1 here)
* CTRL+SHIFT+G to activate the Git pan in the bar on the left
* Enter a message then press Ctrl + ENTER
* The file is now commited locally
* Click on the "..." and select **Push**
* You may have to type you're Git credentials
	* If you get tired read "About entering credentials" below
* You're done!

## YouTubegraphy
1. https://www.youtube.com/watch?v=6n1G45kpU2o
2. https://www.youtube.com/watch?v=9cMWR-EGFuY


## About entering credentials
In a terminal type : git config --global credential.helper wincred
Read https://github.com/Microsoft/vscode/issues/26573

