
## Mordhau CTF

Based roughly off of Th3M4ttman's CTF mod: https://mordhau.mod.io/capture-the-flag

I've redone a lot of the code from scratch. Notable changes:

- HUD now shows time remaining as well as team scores.
- Flag is a weapon you can kill people with.
- Flags cannot be captured unless your own team's flag is at home.
- You cannot pick up your own team's flag if it is at its pedestal.
- Sound cues for when the flag is picked up/returned/captured.

## Make your own map

- Download this repo and stick the "NukeCTF" folder in your uSDK maps folder. If you aren't sure where this is, read the uSDK document and learn how to start a map from scratch. The uSDK guide: https://docs.google.com/document/d/17A2JBqtCwxjYlFttLe_2HU1UJaeaEv4-7veKMXgWOtg/edit?usp=sharing
- Create a new map with its own folder. This will be your CTF map.
- Once you have your map basics set up, you need to reference these CTF blueprints. Your game mode settings for your map should look like this: https://i.imgur.com/UINMvf5.png
- In order for your map to be functional you need to have 2 FlagPedestal instances, each with the appropriate team assigned. This is where the team flag spawns.
