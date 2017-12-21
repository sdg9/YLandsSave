# One time Setup

Find your [YLands save location](https://ylands.com/community/topic/5442-save-file-location/)

1. C:\Program Files (x86)\Steam\userdata\
2. Search for 298610
    1. If there are multiple it's likely the one containing the most recently modified "remote" folder inside
3. For example mine is `C:\Program Files (x86)\Steam\userdata\27090545\298610\remote\SaveGames\STRING CHEESE ISLAND.ylandsgame`
4. Create a shortcut or jot this down for later
5. Clone this github repository your YLands directory
   1. You will need to be able to run `git` from command line (CLI) or a Git GUI client.  The rest of the readme assumes git cli.
   1. Assuming it is not empty you will have to do the following
       1. Run `git clone https://github.com/sdg9/YLandsSave`
       2. Manually move all the files (.git folder (hidden), .gitignore, README.md, STRING CHEESE ISLAND.ylandsgame) from YLandsSave to your YLands directory

# Hosting

## Pull the latest save
1. Navigate to your YLands directory
2. Run `git pull`

## Upload the latest version (after you finish hosting)
1. Exit the game (YLands can be running).
2. Navigate to your YLands directory
3. Run the following
    1. `git status`
        1. You should see it list that STRING CHEESE ISLAND.ylandsgame has changed
    ```
    $ git status
    On branch master
    Your branch is up-to-date with 'origin/master'.
    Changes not staged for commit:
      (use "git add <file>..." to update what will be committed)
      (use "git checkout -- <file>..." to discard changes in working directory)
    
            modified:   STRING CHEESE ISLAND.ylandsgame
    ```
        
    2. `git commit -am "New save"`
    3. `git push`
    
