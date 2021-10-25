# IBringItOn
2. “I BRING IT ON” Task. This task is based on the previous one (“I Can Win”)

    2.1 Add to your project file .gitignore and set this up to hide files with extensions .db, .log, etc. and folders with names ‘target’ , ‘bin’ etc.
	
	 **cd ..**
	 
	 **git clone git@github.com:ViktarKimpel/IBringItOn.git**
	 
	 **cd IBringItOn/**
	 
	 **echo *.db0 *.log target/ bin/ >.gitignore**
	 
	 **vi .gitignore**


    2.2 Create a branch ‘feature’ and make two commits to it.

	**git checkout -b feature**
	
	**echo Agitatis Ultramarini, Dominitis Ultramarini! >song.TXT**

	**git add song.TXT**

	**git commit -m "add first commit"**
	
	**echo Agitatis Ultramarini, Dominitis Ultramarini! Non praestatis Ultramarini, Nobilitis Ultramarini! >song.TXT**

	**git add song.TXT**

	**git commit -m "add second commit"**

    2.3 Merge ‘feature’ branch to ‘master’.

	**git checkout main**

	**git merge feature**

    2.4 Navigate back to ‘feature’ branch and create a file ‘arrows.txt’ with the content as below:The ship glides gently on the waves As day turns into night. Make commit.

    **git checkout feature**
	
	**echo The ship glides gently on the waves As day turns into night >arrows.TXT**

	**git add arrows.TXT**

	**git commit -m "add first two lines"**

    2.5 Switch to ‘master’ branch. Create there a file ‘arrows.txt’ with content as below: One thousand burning arrows. Fill the starlit sky. Make commit.

    **git checkout main**
	
	**echo One thousand burning arrows. Fill the starlit sky >arrows.TXT**

	**git add arrows.TXT**

	**git commit -m "add second two lines"**

    2.6 Merge ‘feature’ to ‘master’ resolving conflict: save all 4 strings in file ‘arrows.txt’ in the same order  how they were added in steps 2.4 and 2.5.

	**git merge feature**
	
	**vi arrows.TXT**
	
	**git add arrows.TXT**
	
	**git commit -m "merge"**