- Logseq github configuration (based on https://github.com/CharlesChiuGit/Logseq-Git-Sync-101/wiki/For-macOS-users)
	- After Git is set and a private repo is created:
	- Go to your local drive and right-click on it.
	- You should see `New Terminal at folder`, click it. If you don't see this option, check [this link](https://www.maketecheasier.com/launch-terminal-current-folder-mac/) to enable it.
	- Type `git clone git@github.com:{your-username}/{your-reponame}.git` and hit enter.
	- If it's your first time git clone something from GitHub, it will 
	  probably ask if you agree to authorized the connection, just type `Yes` and hit enter.
	- After it's done, you should see a new folder with your repo name.
	- Open the folder, there should have a hidden folder named `.git`.
	- Copy&paste the `post-commit` and `pre-commit` in `.git/hooks`.
	- Right click in `.git/hooks` and click `New Terminal at folder`, type
	  
	  ```
	  chmod +x ./pre-commit && chmod +x ./post-commit
	  ```
	  to make those files executable by MacOS.
	- Open Logseq and add the folder with `.git` as your new graph.
	- Open Logseq > Settings > Version control > toggle on "Enable Git auto commit".
		- If you don't want auto-commit to commit in the middle of writing, you can use the [git-plugin](https://github.com/haydenull/logseq-plugin-git) by [haydenull](https://github.com/haydenull) to commit manually by yourself.
	- Type something and wait few minutes to see if what you typed has also appear in GitHub.
	- If nothing goes wrong, you are a happy Logseq user!
	-