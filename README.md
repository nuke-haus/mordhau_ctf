
## Mordhau CTF

Based roughly off of Th3M4ttman's CTF mod: https://mordhau.mod.io/capture-the-flag

I've redone a lot of the code from scratch. Notable changes:

- HUD now shows time remaining as well as team scores.
- Flag can be used as a weapon, however it is somewhat weak. It looks cooler.
- Flags cannot be captured unless your own team's flag is at home.
- You cannot pick up your own team's flag if it is at its pedestal.
- Sound cues for when the flag is picked up/returned/captured.

## Make your own map

I've included the test map i used to test my blueprints. It's ugly but functional. This mod uses a set of custom blueprints that override the game mode, game state, player HUD, and so-on.

Copying blueprints to new folders is really wack, it tends to break a bunch of their references. So if you want to make your own map i think this is the best way to do it:

- Download this repo and stick the "Chasm" folder in your uSDK maps folder. If you aren't sure where this is, read the uSDK document and learn how to start a map from scratch. The uSDK guide: https://docs.google.com/document/d/17A2JBqtCwxjYlFttLe_2HU1UJaeaEv4-7veKMXgWOtg/edit?usp=sharing
- Open the CTF_Chasm level in the UE4 editor and do file -> save as. Save it as your new map name in the same folder.
- Rename the folder your map is in to whatever your map's name is. Make sure you do this via the UE4 content browser since if you do it any other way it will mess things up.
- Rename the shared assets folder in a similar fashion. It should be YourMapName_sharedassets.
- If you did all this properly, you should be good to go... If the blueprints still get messed up then join the Mordhau modding discord (https://discord.gg/wTtjuR) and ask someone for help.
