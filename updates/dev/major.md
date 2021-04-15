## VirtualPE Development updates:

- Start work on SkyFactions (Our first mixed gamemode), between Factions and SkyBlock.
- Added a very unique way of raiding: Cores. (Info at #👀・sneakpeaks.)

**What are Cores?**
- Cores, are essentially a way of raiding. If you have a core, then you can't be raided. If your core get's destroyed, raiding is possible. Try to protect the core as much as possible, fight enemies, and get them away from the core.


**How does a core work?**

To raid an Island you first need to destroy the core of an Island. This core can be upgraded with "Essences" and gets more and more health per Upgrade. After the core of an island is being destroyed the attackers are able to completely raid the base and loot them. The defenders of the base can defend their base too, with traps or other Features. You can also save money in a Core.
If you click on the core of your faction you open a GUI where you can do different things, just as giving it Essences and saving money.

- You can no longer kill the core when you're a member of the island. Same also applies to if you're an owner of that island.

- Fixed being able to leave your own island using /is leave.

- Fixed being able to remove yourself from your own island. These issues lead to consequences. 

- Added custom island area (Thanks to @kewl kenny for this!)

- Fixed being able to kill the core when you're a member of an owner's island, and if the owner of the island is offline.

- Added check to ensure the killer is the same as one of the list of Members from /is members.

- Upon island creation, an end crystal (Core) will spawn upon your island.

- Fixed going through the void when you first spawn on your island.

- Added more details to a player's health with nametags. Displays the following things:
* Current Health / Max Health.

* Percentage, current health dividing it by max health.

* Hearts. Red Hearts means that's how much out of a percentage your health is at. It goes all the way up to 20 to reduce clogging of hearts, but your health can go up to way more than that. The hearts count via percentage.

- Fixed client crashes with the new HP update.

- Fixed crash when breaking/placing blocks from an island that's not yours.

- Added world border plugin!

- Added minions! Finally!

- Added mage minions! How they work:

The mage minions spawn (currently 1) iron golem (Guards) at the same time. The mage minions are used to defend your core. If someone is trying to attack the core, the guards of the core will try to protect it as much as possible. Will you be able to sneak in those destroy-able vibes?

- Due to many feedback, I've decided to make island generating work differently than the previous update. Instead of relying on how much blocks per island, it'll now generate an island and teleport you to a random X and Z coordinate automatically. We decided to do this because raiding was easier than first thought. So I've decided to make island generating random per island, so you could be very far away or further enough from an island. Thanks to @Mitchell for this suggestion!

- Guards will no longer attack the island owner and its members. 

- Added a next spawn timer for Mage Minions, so they spawn once every 30 minutes (will spawn atleast 2 per spawning in the next update or so).

- You can no longer attack your own/island's guards (Iron golems).

- Fixed a bug, where core and the player spawned somewhere near the actual spawn location, and not exactly where the spawn located was meant to go. Now, it'll spawn you to its correct positioning, including cores, and the sender. Along with this, it'll also set the spawn per island located to where it's meant to go when you use /is tp.

- Added new minion: Essence.
Essence Minion, is a minion that lets u claim an Essence every 12h. You can upgrade the Essence Minion with more Essences.
There are 3 Levels on the minion.
To Level from 1 to 2 you need 3 Essences.
From Level 2 to 3 you need 5.
Level 1 has 12h Cooldown
Level 2 has 8h Cooldown
Level 3 has 6h Cooldown.

- Added Upgradeable cores. Thanks to the feedback, this is now a thing. We may change how upgrading works soon. But for now, this'll be the design and what it'll look like.

- Finally added social spy to the server!

- Added new API function: getSocialSpyPlayers(). This function will retrieve all online players using socialspy.

- All chat messages will now appear even if the database is down directly to discord.

- You can now talk in /sc, even if the database is offline.

- You can now talk publicly from in-game to discord whilst the database is offline too now. Before, this wouldn't of been a thing.

- #👀・last-seen, #⚕・staff-commands and #🤖・player-commands now appear messages even when the database is offline.

- We've fixed the interaction spam to do with Interacting with vanished items (Staff mode), so you should no longer receive any spam when clicked on once.

- Added new command: /socialspy AKA /ss - Socialspy commands.

- Fixed crash when opening the upgrade system for Essence Minions.

- Will now state if the level and cost is at max level, instead of continously appearing a level you simply can't access, possibly due to the maximum of levels you can go to.

- Fixed incorrect message bug when on the selecting a trap screen. It'd state already unlocked if you haven't unlocked it yet, and will do the same vice versa.

- We've completely got rid of the old 1 minute, 1 second stuff for #👀・last-seen, and made a new API for it which should work a lot better. Alongside this, the restart time system has been completely rewritten to make it better.

- This may look the same, but I've just made a few code improvements on the restart system.

## Vanishing

* We've completely rewritten Vanish time system. We've added short signatures, such as 1s for 1 second, 1m for 1 minute.

## Other Changes
* We've  made some changes to #👀・last-seen and other minor features, such as If a minute, second, hour, or day is at 1, it won't display the "s". As that's grammatical incorrect, and shouldn't be used all the time. This is now correct.

- Fixed crash when loading scoreboards.

- We've completely rewritten scoreboards, once again! They now look 1000x better than before.

- Added Vanish Support to the new scoreboard system.

- Fixed issues where the old scoreboard system would interfere with the new scoreboard system (In terms with vanishing).

- We've added a lot of things to nametags! Such as:

* Device
* Ping
* Hearts
* Faction name and faction rank.
* Player rank

- We've added our own Factions System!

- Added Activity Points. 

How they work?
- Activity points, is a currency system for Factions, where you can do certain subjective's to receive Activity points. There are a few ways you can get Activity points. The ways are:
* Mining - 0.5 per break.
* Placing - 0.25 per place.
* Being active on the server. 0.05 per second
* Killing an enemy - 100 per kill.

You can also use Activity points in /f shop, where you can buy certain items with Activity points.

- Added spawners in /f shop! Yay!

- Fixed Money Notes not being money notes, and would instantly give you the money from /f shop.

- We've made Guardians 1000x better than before! AI should now function, slower, but better. It'll get the job done.

- Guardians now regen hearts every tick. Can you kill them and steal the cores!?

- Added /upgrade - All Island upgrades.

- You can now increase your island size by 50% (+50 blocks per level) using /upgrade menu.
