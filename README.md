# Project Overview 📎

This project is a bot application for use with the platform Discord.

This application was created using the Discord.py API.

This Discord bot can create Wordle games which users can play in their own Discord servers.

Available words are stored in the words.json file, which can be edited if wanted.

Additionally, the program creates a wordlebot.log during runtime to help debug issues.

---

## Commands ✏️

**/sync:** 
    
    Permission: Administrator

    Description:
    Syncs the script commands to Discord.

![sync example](images/sync.png)

**/startgame:** 
    
    Permission: Member

    Description: 
    Creates a new Wordle game with 6 attempts. Words are taken from the words.json file. Cannot be called if there is currently an active game.

![startgame example](images/startgame.png)

**/guess:** 
    
    Permission: Member

    Description:
    Allows a user to submit a guess to the active Wordle game. Guesses must be only 5 letters long and must contain only alphabetic characters.

![guess example1](images/guess1.png)

![guess example2](images/guess2.png)

---

## Developer Usage 💻

### Copyright: 
- This code may be used for commercial or personal use, as long as the author is credited.

### Other Notes:
- This code uses an unpublished .env file to store the Discord Bot Token. If you are using this script as reference, make sure to create your own .env file with your own Bot Token in it, or simply replace the .env usages with a constant.
- Since the commands are not synced globally, any guilds (servers) you wish to use your bot on needs to have its guild id loaded in the guilds.json file.
