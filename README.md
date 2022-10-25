# cheeze42s_KHCOMrandomizer
The above LUA script is a recovered copy of cheeze42's original Kingdom Hearts: Chain of Memories randomizer for GBA.

It was originally removed from his Github account, but has been reuploaded with permission from the Author, here.

I won't be making any changes to the original file, as I want the original copy to stay in tact. 

It is as close to being unedited as I remember, and is functional, however it appears to be in a WIP state at the time I downloaded it.

# Instalation 

It seems to be intended for the Bizhawk Emulator. 

(I teseted it on version 2.8-Windows and 2.6.1-Windows. It should work on newer versions, however I cannot personally vouch for it)

To use, 

1. Download or copy all the text from the .LUA file, and save as a `"Something.lua"` under `Bizhawk > LUA > GBA`.
  If there is no GBA folder, that's fine. It will ask you to point to the file anyway so just save it somewhere you'll remember.

2. Then open Bizhawk and Load your Kingdom Hearts: Chain of Memories ROM. `Kingdom Hearts - Chain of Memories (U)`

3. From the title screen (generally anywhere but titlescreen is safest...), go to `Tools > Lua Console` in Bizhawk.

4. Once it has opened, make sure no other scripts have been loaded, or conflicting, then go to `Script > Open Script` 
  In the new window, select the `.Lua` file you saved earlier. 
  
5. Make sure you get a message in the `Output` side of the Console that reads `"Seed: xxxxxxxxxxx"`

6. You're done! You can enjoy a randomized version of Chain of Memories now! The script should only run once and stop, so you can close the Lua Console when you are done. **However, if you close Bizhawk from this point, you will lose your saved game and randomized seed. **

7. (Recommended) I highly suggest you write down or copy your seed to a file, or a notepad, as there is no *easy* way to load the seed if you crash/close Bizhawk.

# Loading a Seed 

If you crash or close Bizhawk, all of the ram values for your seed get wiped and the randomization is gone...

However, you can have the script reuse your seed again to "place all the cards back" and keep playing after you close Bizhawk. 

1. Copy your seed number EXACTLY as displayed. So if it says `"Seed: 12345678"` write down `"12345678"`

2. If you would like to have the Script use the seed again, open the `.Lua` file with a text editor, and scroll to line **93**.
  It should say `seed=0`. Zero tells the script to *make* a new seed every time you launch the script in the Lua Console. 
  
3. Replace `seed=0` with your seed number. In this example your seed would be `seed=12345678`.

4. Reopen Bizhawk, Load Chain of Memories again, and go to `Tools > Lua Console`.

5. Select the `.Lua` file again, just like before.

6. Done! Your seed will be rewritten to the game. To verify, make sure that the `Output` in the console reads `Seed: 12345678` (or whatever number you have).

7. You can load the game from an in game save, and should be good to go. 

8. (Optional) To go back to new randomized seeds, reverse these steps and set `seed=` to `0` again. 
There are a few things to note, before you play however...

# FAQ / Things to note...

* You should be able to load and save the game like normal, without much trouble. Just remember to have the script load your seed every time you relaunch Bizhawk/reset. Your ingame Deck is saved like normal, but not the randomization on card rewards. 

* If it looks like your cards aren't random in the start, wait a bit and keep playing. The tutorial fights (with the hooded figure/Leon fight) are not randomized. The game keeps extra sets of decks with specific cards for those fights, and nothing will look different or be changed for those.

* Play up until you fight the first heartless in the save room, there your "normal/default" deck of cards are loaded. Those should look different.

* World Cards are untouched. (I think)
  This means that your reward for encounters and door requirements should all be the same. (Should...)
  
* The cards are randomized to some extent but not entirely random. You'll see most cards shuffled into their own pools, and only some will mix into another pool. (Enemy cards are generally shuffled with enemy cards. But Attack and Magic Cards might cross into each other's pools.)

* As far as I know, there is no "logic" designed into this randomizer, like other randomizers. None is really needed as this pertains to just battle cards, and you can get through most fights in the game, even with weird or *unique* combinations of cards. The whole game (should) be beatable. 

* No changes to Riku's Story (Reverse/Rebirth). At least non are intended. 

* You WILL have the extra bonus cards from beating Reverse/Rebirth, in your card pool. You might see cards you never knew where originally in the game!

* You might get more initial cards in your "starter" deck than you have Card Points to hold...
  * Because higher tier cards cost more, you might start with a 400 CP deck, but only have 375 Max CP to begin the game.
  * In this case, when you open "Review Decks" to look at your cards, you will get locked in that menu, as the game only checks when you go to leave, if you are under your Max CP Limit. 
  * This isn't so bad, as you can just remove cards from your deck until you are under Max CP again, like you would in a vanilla game.
  
* This script seems to be a WIP still, I'm unsure where/when you might run into a crash, however I have not found one...yet. 

# Credits / Thanks

Thank you SO MUCH to cheeze42 for writing the script so long ago, and also giving permission to reupload it. 
I asked if he would be fine sharing it and, you can see in the **Issues** tab on this Repo, he gave his blessing so the world may see it. 

**If you want to do other stuff with the script, go for it. However I ask that you too, pass on the credit to @cheeze42 if you do. 
He IS the original author of the script and deserves the praise here. I just uploaded it after he had deleted the original. ** 

(If you have any questions or comments, please go ahead and make a new "Issue" here on github. I am new to Github, but will try to respond to what I can, or what I understand about the script. However, please understand that it is also a "What you see, is what you get" scenario. I don't know the intention behind any of the code written, I just had the spare copy reuploaded for the world to see.

I will be making few changes to the Original Code. I have added a branch label "Original Recovered Code" for the original project as I found it, the Main Branch and any modified branches will be changes I make to the code.) 


