# Purpose
Allow anyone to host YLands with a few simple commands (details in Hosting section)

It requries everyone who hosts to upload their file back to github when complete with a game session.  If you forget and people play a new game session with a different host in between, your session will be lost.

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
Navigate to your YLands directory and run
1. `git pull`

## Upload the latest version (after you finish hosting)
Exit the game (YLands can be running), navigate to your YLands directory and run
1. `git commit -am "New save"`
2. `git push`  

#2 should take a few seconds as it will upload a 18mb file
    
# Fringe benefits
- If something bogus happens (one of our computers blows up, Anthony joins and steals all our goodies, etc) we'll have a restore point for every game session.
