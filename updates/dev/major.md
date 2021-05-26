## VirtualPE Development updates:

## This changelog introduces a new and complete Core revamp, along with: Major API changes (API BC), and many changes with the concurrent server.

- Start work on SkyFactions (Our first mixed gamemode), between Factions and SkyBlock.
- Added a very unique way of raiding: Cores. (Info at #👀・sneakpeaks.)

**What are Cores?**
- Cores, are essentially a way of raiding. If you have a core, then you can't be raided. If your core get's destroyed, raiding is possible. Try to protect the core as much as possible, fight enemies, and get them away from the core.


**How does a core work?**

To raid an Island you first need to destroy the core of an Island. This core can be upgraded with "Essences" and gets more and more health per Upgrade. After the core of an island is being destroyed the attackers are able to completely raid the base and loot them. The defenders of the base can defend their base too, with traps or other Features. You can also save money in a Core.
If you click on the core of your faction you open a GUI where you can do different things, such as giving it Essences and saving money.

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

- We've added a new channel: #👊・punishments. This channel will log all punishments, made to the server automatically. If you: Unban a user, ban a user, mute or unmute a user, it'll now state this in #👊・punishments. Please keep in mind - The reason why we still have #❕・punishment-format and #📝・punishment-logs is because when punishing a user, you still need to provide proof of that punishment. The punishment system can't automatically do that for you, hence why we have to do it manually.

- All bans and mutes are now through a MySQL Database. This means once we add more servers, all punishments will be through the network (All servers), not a single server.

- Added new command: /ban

- Added new command: /mute

- Added new command: /unmute

- Added new command: /unban

- We've fixed many bugs relating to command exploits, and being able to use certain commands whilst muted.

- We've implemented a brand new system, where if you join the server, you need to talk atleast 1-2 times for the chat to display. This is because it's attempting to load your mutes and bans in (if any). If not, it'll allow you to talk. The message will say "Try talk again as we are checking for your mutes". Once spoken, it'll either cancel the chat event for the specific player (if muted), or it'll allow you to speak. We do this because of MySQL: MySQL performs a async task, which takes a few miliseconds - 1 second to complete. Because the PlayerChatEvent is an instant event, we can't actually uncancel the event when you join, as if we did that, then there would be a lot of bypasses to the mute system, and that wouldn't be good. My goal is to limit the bypasses for mute system.

- Fixed Mute messages displaying incorrectly.

- Fixed ban messages displaying incorrectly.

- Fixed mute command from kicking you.

- You can now mute, and ban offline players also.

- We've made bans and mutes slightly better!

## How they work?
- You can use the command: /ban <player> <type> <time> <reason>

[type] is the type of ban/mute you'd like to use. Valid ones are: temp and perm. If using perm, you only use /ban <player> perm [reason]. If using temp, you can use /ban [player> temp <time] [reason]

[time] - You can use time formats like d, m, s, etc. d means Day, m means minutes, and s means seconds. We also have premade timers for you, so if you want to ban or mute someone, you can use the valid reasons, as described in /ban or /mute usage.

[reason] - Just put a reason for the punishment. It needs to be valid, or it won't go anywhere, and we'd simply unban/unmute them.

- Fixed ban messages from displaying incorrectly.

- Fixed mute messages from displaying incorrectly.

- Fixed mute command from kicking you from the server.

- Added a new system, where if you join, you have to chat or use commands atleast 1-2 times. This change is because of MySQL - How MYSQL works for us, is async task. This basically prevents any server strain whilst it works in the background. That's the main point of a async task. The reason behind this change was because the Player Chat Event is instant, so if someone types, it'll instantly activate the event. This is a messy hack to prevent mute evaders. It'll simply check to see if you're muted or not. If you're muted, it'll rightly state so. If you aren't, you can chat freely. The difference between the join event, and the chat event is simple - PlayerJoinEvent can be delayed using a async task. Because when you join, it'll allow you to use other things in the background, like async task. With PlayerChatEvent, it activates instantly. You can't use async task using it to cancel the event, as that's not possible. So writing this hack prevents mute evaders in so many ways. I know this may be annoying to most of you, but if there was any other alternatives, I'd simply do it. 

- Fixed bans and mutes not saving to MySQL Database.

- We've added a brand new system for Aliases, which has more than one alias option. If you use /alias <player>, it'll state: "IP, XUID, Self Signed ID, Device ID, and Client Random ID. "

- You can now alias offline players finally!

- We've implemented a new network methoding stage! How it works:

So currently, this doesn't affect anything, but once more servers get added, you will see a good difference.

## HOW IT WORKS
- We are adding our servers to MySQL. As a good thing about MySQL, is you can actually make a multi-server with it. We have created our very own MYSQL Database for our servers through out the network. Those affected will be/are:

* Total Online Players - When we add more than one server, you can tell the Online Player Count and Max Player Count is higher than previously. No, this isn't fake slots. This is because we managed to link our server slots, and max player slots to the MySQL Database, which displays more players / max players than usual: It displays total amount of players online and the total max players online, if +80. For example, if there was two servers, and they were both 80 max slots,
the database will recognize this, and display 160 max player slots instead of 80, as it's counting the max player slots of both servers. 
* Displaying if the server is online. Returns true if online, returns false if not. 

* Displaying if the server is in maintenance mode. Returns true if online, returns false if not.

* Displays server IP.

* Displays Server port (The port is automatically checked from the server.properties server-port option.)

* Server Alias: Currently, this only includes the server name. We may make this with some use soon.

* ServerName: The server name it displays in.

## NOTE
- When using boolean to return true or false, MySQL has it differently, so they're known as "TinyInt". Essentially, it's a 0 or 1 number (0 for false, 1 for true). It converts a boolean into a tinyint (AKA either 0 or 1)

- We've completely revamped some Network::class API's.
- 
- Network::getServerName() no longer relies on the server's MOTD. It'll return the actual name of the server. This is so we can add our own MOTD.

## CURRENT KNOWN ISSUES WITH THIS UPDATE
- Sometimes the Maintenance mode would be set to true or false, even if it's not whitelisted. This would only occur when you're using the command from another server after that specific server is being whitelisted/unwhitelisted.

- We've completely rewritten how island generation deletes an island after using /is restart.

- /is restart now makes your island brand new, and deletes the old island. Before, it just kept it there like nothing happened. 

- Fixed some commands not working as intended. The fix, was to use ./ instead of /, but this should now be fixed.

- Disable Network Core if server name and ip is invalid.
- Added new feature: Envoys.

## How does envoys work?
* Envoys, are chests that randomly spawn through out your world. Because we're that unique, we've decided Envoys are going to spawn in the same world as the islands are in.
* We may also plan on making a lot of big changes to Envoys in the near future.
- Added command: /envoys - With this command, you can track down each envoy and their positioning, using Coordinates.

- Timer for Envoys till despawn is now 15 minutes.
- Fixed spawners from not clearing and deleting whilst a player uses /is restart during the process.

- Floating texts from spawners also now delete, instead of appearing still.

- Fixed the aftermath of /is restart not regenerating the new island properly.

- Completely cleaned-up a bunch of junk with commands being in the wrong classes and folders.

- Most command's autofill should now be fixed. Issues with this would be things like commands appearing even if you don't have permission to use it.

- Made a new folder: Moderation, which has all the moderation commands for staff.

- We've completely moved all of the moderation commands to essential\command\types\moderation, and moved a few older moderation commands to that folder also.

- Fixed /spectate command from breaking, and didn't output the correct command usages.

- Check if the server is online when transferring a player to a specific server. If it returns true, it'll skip that check. If it returns false, it'll give you an error message.

- Check if the server is whitelisted when transferring a player to a specific server. If it returns true, it'll skip that check. If it returns false, it'll give you an error message.

- Added the new and updated WaterDog support for Transferring servers. It'll use the $player->transfer() method, whether you use waterdog or not, it'll still use the same transfer method. If you're using Waterdog, then the Transfer function will go to waterdog's transferring method. This change is useful so we don't have to change anything majorly when switching to a proxy in the future. 

- Added new command: /transfer - This command will allow you to transfer to any of our servers within the network. 

- Fixed users not being transferred properly, and getting the "Disconnected from server" bug during its restart.

- Cleaned-up useless parmaters for BuildMode Command, and made it work like the other commands.

- Fixed crash when transferring to a server they're banned from.

- Fixed crash when transferring to a server they're not whitelisted on.

- Fixed a crash when transferring to a server that is not online.

- Exploding a spawner will now always drop the spawner that had been exploded to, rather than only sometimes occurring.

- Fixed Floating text from Spawners causing issues with it not disappearing when it explodes.

- Fixed an issue where spawner levels would reset. This update prevents this from happening.

- Fireworks now launch above the Envoy chest. This is useful for knowing around where it is.

- Added custom names and lores for spawners.

- Fixed client crash when using /is restart command.

- Added /tags - Allows you to open a UI, where you can select your tag (depending on if you own the tag).

- Envoys has been extended, in terms with functionality.

- Fixed an issue, where envoys would only spawn if a user is online.

- Added a brand new Envoy island, finally! Yay.

- Fixed server crashes when chest tiles were spawned in areas where chunks weren't loaded. This is a hacky fix, and should be for the duration.

- Added a brand new feature called "Envoys platforms". 
- 
## How does it work?
* This feature allows the server to spawn a platform below where the envoys are.
* This is so items that try to fall into the void will be saved for 10 seconds.
* You would then need to get the items from the envoy that were on the platform within 10 seconds, otherwise
* it'll disappear. This is useful for if you don't want to place blocks around the envoy island, as it'll place it for you.
- Added a boss bar timer to Envoy platforms counting down from 10 to zero, which then will despawn.

- Fixed Boss bar percentage from always being 100%. Now, it goes down from 10 to zero.
* The reason why this bug occurred, was because with Boss bar percentage,
* Percentages work by making the percentage (1-100), and then dividing it by 100.
* For example, 50 percent would be 0.5, 100 percent would be 1, etc.

- Reduced the platform size to reduce lag.

- Added new command: /flyshop.

## How it works?
* You can actually buy fly time. Fly time, is a temporary solution, where you can increase your fly limitation.
* Using the command /flyshop, you can buy fly time, as stated in the FlyShop UI.
* When activated, it'll state how long your flight time will be.
* Keep in mind - You can add onto another set amount of fly time minutes.
* For example, if you already have 5 minutes as your fly time, you can add onto another 10 minutes, which would be 15.
- Vanished player's /fly will no longer disable when fly time is over. Flight will be disabled if the user isn't vanished.
* Great for moderation purposes.

- Added updated Factions support for Ranks and chatting.

- Removed health and max health status to the Tip message. This is because it was clogging up general uses,
* and we can't have that.

- Added API methoding for Bossbars. Using Network::getDiverseBossBar(), and Network::getBossBar() API methods.
* Another way to obtain them is by using DiverseBossBar::get() and BossBar::get().

## What are the difference between DiverseBossBar, and Normal BossBar?

* DiverseBossBar: Sends different data per player.
* BossBar: Sends the same data per player.

- Removed Network::isGamemode() API function because it will now always return true, so the best option is to remove it entirely.
- Removed the following API Methods:
* Network::onEnchant()
* Network::isEnchantmentServer()
* Network::isGamemode()
* Network::updateScoreboard()
* UpdateManager::updatePublicScoreboard()
* Network::timeToSeconds()
* Network::isScoreboard()
* Core::isLobby()
* Core::loadInventories()
* Core::addInventory()
* Core::isLimbo()
* Core::getInventories()

- Renamed the following API Methods:
* Network::number_format_short() -> Network::shortNumber(), and improved the function.
* Network::calctime() -> Network::getFullTime()
* Network::timeFormat() -> Network::getFullTime()
* Network::timeToSeconds() -> Network::getFullTime()
* Network::isLobby() -> Network::isLobby() - Returns bool instead of string.

- Addded the following new API Methods:
* Network::getTotalPlayers() - Totals all of the players online function, combined.
* Network::readURL() - Reads the link from the URL, can be used for file transfer purposes, code sided.

- Network::isInstalledPlugin() now returns Network::getPluginName(). The difference with Network::isInstalledPlugin(),
* is it checks whether the plugin is null (whether it's installed or not).

- Made Network::isLobby() return a string parmeter, rather than returning the server name.

- Added those with Server::getInstance() to be Network::getCurrentServer() for API flexability.

- Made Network::isEventServer() return a string parmeter, rather than returning the server name.

- Fixed Network::getOnlinePlayersWith() returning a Player::class objective from not being found due to a typo.

- Network::isLobby() now returns the Server::isLobby() instance.

- Fixed crash when respawning.

- Increased world border size to 20kx20k

- When at the end of the border, it'll now teleport you to your island (if you have one).

- When at the end of the border, it'll now teleport you to the same Y Coordinate, but different X and Z coordinates. (If you don't have an island)

- Fixed an issue, where players couldn't fly whilst in creative mode.

- When in combat, a stone block will spawn below your feet if on the 25 Y Coordinate.

- Fixed being able to upgrade spawners that aren't even yours.

- You can now only use /is restart if you're the only one on your island.

- Island Protection now relies and supports higher island sizes, leading to more protection depending on island size.

- We've updated our staff mode system.

## HOW IT WORKS?
* Staff mode, is a moderation feature. We've updated it masssively.

* Added an experiemental feature: Replay Mode. How it works:

** You can now record other players and entities, play back the recording, and save a recording. All in just staff mode.

* Because we have too much items in one inventory space, we've decided to now introduce Pages.

* There are 3 items per page. Papers are pages, and you can go through them all in just over a page. Either click Next page

* to go to the next page number, or previous page item to go to the previous page number
- Fixed not being able to open chests after you've destroyed the core.

- You can now craft a working shield!

- You can now use the enchantment table to buy Vanilla enchantments using lapis, as you would normally in vanilla.

* We will be making vanilla enchantments hard to get. The only way you can get it, is from an enchantment table, and we will make ways of getting things like enchantment table, etc soon.

- You can now use the anvil to repair your items!
- Fixed crash when upgrading your island size.

- Fixed trees not being able to be broken because the core was too close to it. It'll now allow you to break leaves and logs no matter how close it is to the core.
Keep in mind - Placing logs and leaves near the core will not allow you to - This is to prevent abuse.

- We've made a few changes relating to the core, and how it destroys.

- The core destroy sound will now always occur whenever you break a core. Before, it'd only make the sound effect when the core's player is online.

- The server will now broadcast whenever a core has been destroyed.

- Added offline support for retrieving the player's name from the core objective, which then can be used for destroyal messages.

- Made a ton of improvements and implementations to how /is visit will work.

## How it works?
* Whenever you type /is visit <player>, you will be known to not being able to break blocks, place blocks, interact with anything, destroy the core, attack entities and players, and add buckets to the island.
* This is logical behavior. Once you either get teleported to spawn, or teleport to your island, visitor mode will be disabled.
* During the visitor mode being enabled, you won't be able to turn on coordinates using /xyz on. The visitor mode is very limited, to prevent abuse.

- Renamed command: /is lock -> /is private.

- Messages for /is private on has been changed.

- Messages for /is private off has been changed.

- An warning message will be issued to you upon using /is private off, so you know what risks are involved when making your island public.
- Fixed having to chat 3 times before you're able to speak. It's now 2 tries. One which will be the message to type again, and the other, you will be able to talk.

- Fixed /is restart from being able to delete other people's islands.

- You can only use /is restart when on your island. If you use it on islands that aren't yours, or not in a valid island world, a error message will popup, in chat context. Stating you can't use this command here.

- Added new command: /is help

- Fixed crash when only inputting /is help.

- You can now use /is to bring the /is help usage. More easier and better understanding than it was previously.

- Leaving the server whilst visitor mode is turned on will now teleport you to spawn before it counts you as left the server.

- Server restarts whilst visitor mode is turned on for player(s) will now teleport them to spawn before it counts the server as disabled.

- Fixed Visitor mode being disabled when you go into the void on another user's island.

- Fixed players being able to attack visitors.

- Fixed bug, where you'd sometimes go inside blocks upon island generation. The reason for this cause is because

* It releases the player as soon as the island generates. This takes from 1-3 seconds to generate. And before,

* players were released from their position as soon as the island generated. Now, the player will be released from their current position after 3 seconds of island regeneration

* to prevent any entity colliding with blocks issue.

- Fixed /is restart relying on the Last X and Last Z, so if the last player created their island using /is create, and another

* player uses /is restart, it'd clear the last player's island that used /is create or /is restart on.

* Now, it relies on the specific sender's X and Z coordinates within the spawn positioning.

- Fixed some parts of the island not deleting properly when using /is restart.

- You can no longer interact with enchantment tables whilst in visitor mode or if the core hasn't been broken yet.

- Removed Less click interaction spammy messages.

- You can no longer bypass being frozen by using /is restart.

- Added Freeze Support to /is restart releasing the player.

- Completely changed SkyBlock Commands messages to make them look better, instead of the plain white text.

- Fixed /is kick from giving an error to the player that got kicked from the island.

- Added a new display system: Fuel.

## How does Fuels work?
* It's nothing too exciting, except it's a way of knowing the fly time. Though we did have this before, we never gave it a name.

* Once the fuel get's low (1 minute before expiry), it will state you're running out of fuel.

- Renamed command: /flytime -> /fuel.

- Updated Fuel Form UI to be more specific about what fuel is in the server's case.

- Make villager sound when you're low on fuel!

- Updated Fuel message to make it more realistic.

- Added our very own Cooldown API (Also publicly available too)

- Added the following API Methods:

* Network::isCooldownActive(): Checks if the cooldown for the given player is active. Returns true if active, returns false if not.

* Network::hasCooldownTime(): Checks if the time set is over. Along with this, you can set a timer for the given player.

* Network::canUseItem(): Checks if the item can be used to interact.

* Network::setCooldownTime(): Resets the cooldown timer.

- Fixed not being able to place blocks.

- Added brand new minion: Raiding Minion. 

## What does this minion do?
* This minion is a raiding minion, allowing you to break blocks in a certain radius,

* which can be used to break into somebody's base. Maybe if they have an complete obsidian base, or something that's pretty OP, and can't be raided with anything.

* This is where the Raiding minion comes in. You activate it, and watch it start destroying the wall from the base.

- Raiding Minion no longer breaks things like chests, which would then be lootable.

## HOW IT WORKS?
There's 3 different levels of the Raiding minion.

It's a minion or entity you can place which breaks a certain amount of blocks in a certain direction.
The minion cannot break any blocks assigned to the core, neither any chest or things that can be looted. You cannot loot as theres still the protection of the core.

## Blocks and Levels
A raiding minion has 3 different Levels. The higher the further!

## How far tho?
* Level 1 - 15 Blocks for 30 Essences
* Level 2 - 18 Blocks for 60 Essences
* Level 3 - 21 Blocks for 90 Essences

## What happens after raiding the base?
- Well, they simply break. They do not disappear, no you can pick their Pieces up! Essences and iron blocks!


## What does this minion drop?
You can obtain 2 Essences and 5 Iron blocks from them dropping!


## How do you obtain them?

- You can craft it using iron blocks and essences, which will come hopefully in the next update!

- When the raiding minion activates, everyone that is in your island, that is online, and the island they're trying to target, will be alerted that they're being raided, and to warn those involved.

- Fixed being able to break blocks outside of the island border.

- Fixed being able to place blocks outside of the island border.

- Fixed being able to interact with items/blocks outside of the island border.

- Fixed being able to place buckets (Water + Lava) outside of the island border.

- You can no longer place raiding minions in islands you're apart of.

- You can no longer place raiding minions if you're not in any of the player island's.

- Added new command: /is description - Allows you to set a description of your island.
- Added Island titles support.

## How it works?

* So there are two types of titles?

1. Island Title
* So when you're nearer to an island, it'll state what the island is called, and the description of the island you're going towards.

2. Wild Title
* When you're out of the island's border, it'll state you're in the wildness.
- Added Groovy bot to the discord server, thanks @Bubbly for this!

- You now teleport to the server spawn if you fall into the void, and in the wildness.

- Changed up how teleportation cooldown works.

- We're now using: Network::getFullTime() for seconds, rather than using its own timer for things like /spawn

- Removed useless imports.
- Added new class: CoreInfo. This class will be the main course of information, provided to the plugin for either future use or something that's already being used.
* CoreInfo can be used for future things (Like VirtualPE update versions, and what the next version will be.

- Saperated all moderation related stuff, and made it a saperate listener class.

- Saperated all Networking related stuff, and made it a saperate listener class.

- Added Anti Auto Clicker. Instead of it actually kicking, or banning you, it'll just send out a message to all staff members.

- Added new command: /changelog

- All changes will now be directed via /changelog, directly in-game. We may post some updates on discord also.

- The console username now outputs as Auto Detector, in case of any future anti-cheats that provide custom banning system.

- Fixed being frozen whilst you are leaving the server from giving you an error.

- Updated Frozen's ban system.

- Leaving after you were frozen now bans you for 7 days, and not permanently.

- We've finally added our own Updating system.

## HOW IT WORKS?
* When a new version releases, it'll state this when you first join. Essentially like any other auto updaters, except it isn't deemed as an updater.
* It's basically an updater for the /changelog command. Once a new version releases, it'll state all the information you need, and will give you a book.
* Once you either type /changelog or tap the book on the ground, it'll set your state to "Read latest changes", which will then display There is no new updates available upon next join.
* Because we have a new class: CoreInfo, this makes it so we can update the versions ourselves, without dealing with configuration mess, and less customizability as to what I can do.

- Fixed Chest from going in an incorrect direction upon placed whilst in vanish.

- Vanish chests are now trapped chests, instead of normal chests. This fix was made to prevent conflictions.

- Vanish chests now go in the correct direction.

- We've added more items support to Vanish chests.

- You can no longer break normal chests whilst in vanish, to prevent abuse.

- Fixed crash when joining the server if the database is offline.

- Added even more Database offline support for player joins/leave, comparing versions, and more.

- We've introduced a brand new Discord system called "VirtualPE Game Side". Well, that's the category name atleast.

## How does this work?
* So we have a new channel on discord called: #💻・console
* In this channel, we have everything, to storing errors (Not an error message, but an error information that occurred),
* Storing player joins/leaves, staff and player commands, broadcast messages, made from the server to discord,
* Server restart time, and basically anything that logs the server.
* This is more useful for us higherups so we can determine what is going on without actually going on the server.

## API Logics with this
* Well, thanks to our Networking::class, we can broadcast a public message, use Server::getInstance() for broadcasted messages, and we can make it so it logs to discord.
* By using Network::broadcastMessage().

- Fixed color coding font issues from discord's side - Upon join/leave.

- Fixed crashes when opening a vanish chest. This was because some items were causing crashing difficulties, either because it's unknown or isn't yet implemented into pocketmine.

- Delay each onEnable() state message.

- Delay each onDisable state message.

## Why did you do this?
* I did this because before, onEnable() and onDisable() state would randomize each message in a random order. We use sleep(1) upon onEnable() and onDisable() inbetween log messages so it can send out in the correct order.
* You could say this is a type of code hack to prevent messages being randomized, when sometimes it wouldn't make a lot of sense.

- Fixed duplicated chat messages, made in #💻・console.

- We've removed the following channels in VirtualPE discord server:
* #🗣・ingame-chat, #🚔・ingame-staffchat, #⚕・staff-commands, and 🤖・player-commands.

- We've renamed the following channels in VirtualPE Discord server:

* #👀・last-seen -> #👀・staff-activity

- We've made some improvements to how a user chats, and uses command.
* Because we've removed a ton of channels that weren't needed, I've decided to implement a way to display if the user is using staff chat or not, same goes for commands (In terms with if they're using socialspy or not.)
* That way, it's a lot easier to over see the situation and chats.

- We've renamed the following chat messages sections/titles.

* Last-seen -> Last Active.

- We've also made improvements to #👀・staff-activity. Here are the following things that were improved on:
* Instead of appearing as 0 seconds, it'll now state that they just logged on/off. This is to prevent many confusions. Thanks to @TableFungi#5578 for bringing this to my attention!

- Fixed an issue, where the server would take a few seconds to actually kick all online players from the server.

- Added Death, and respawn messages to Discord logging.

- Added color coded death messages for in-game!

- Added a new function: Network::removeCode().

* This function will delete any color coding material. How this works, is:

* If the & symbol is used for color coding, it'll convert that to an § symbol, which will then clean any § symboled message using TextFormat::clean, which basically deletes any sort of coding material with an § symbol.
* We do it this way because it doesn't detect &, so we have to do that ourselves.

- Fixed /burn command from giving you an error if the database is offline.

- Added Envoys Status, which will display how many envoys have been spawned, which updates every 6 minutes. (Discord side only)

- Added new Discord embed titles for anything that's not related to Sender sending the broadcast message.

- Fixed a /burn permission bug issue if the user was opped.

- Fixed players being able to use /burn if they don't have permissions.

- Fixed envoy island not spawning in the chest properly.

- Fixed not being able to break all envoy surrounding blocks.

- Fixed being able to break and place blocks in an area where there isn't an island found.

- Fixed placing spawners to make them stack from not updating the Spawn timer. Before, you'd have to wait until the timer was set to zero, which would then update.

- Fixed duplicated floating texts with spawners.

- Increased default spawner time to 5 minutes.

- Fixed breaking spawners when you're in visitor mode or do not have access to an island, the floating text would disappear for a second.
* This has since been fixed.

- Removed the WorldBorder.

## Why did you remove the Worldborder?
* We removed the World Border because of how easy it could've been to collide with another island's coordinates.
* We removed World Border to ensure coordinates are from 0 to 500k from X and Z. That way, it'll be a lot less conflicts between Island coordinates, and random X and Z coordinate.

- Island creation/Restart now goes out from 0 to 500k X and/or Z.

- Fixed error upon onDisable() with Saving the Server Management side via MySQL.

- ServerManager now saves if the database was online at that given time. This is to prevent errors.

- Fixed conflictions between the same spawners if not stacked. 
* Before, whenever you place a spawner down, it'd show the same Spawner level, alongside the cost as the previous placed spawner.
* This would then only occur whenever you have one of the same spawners, but in different stack.
* Now, it'll use Random() ids within the spawners, as an NBT Tag to prevent colliding between same spawners.

- Fixed crash when placing a spawner.

- Fixed place of spawner from delaying the floating text addition to the player. Now, it'll do it instantly.

- Fixed bug, where you could stack spawners in islands that aren't yours or apart of.

- Envoys now have a timer of 30 minutes.

- The server now spawn 15 envoys at once, every 30 minutes.

- We've reverted the change where spawner levels would save when you break them.

## Why did you make this change?
* Because it would've been buggy, and more bugs could occur with this being enabled.

* Things like: Conflictions could also take place, in which I'd rather not have, for abuse reasons.

- Fixed crash when you use /is create - Because coordinates were too far.

- Envoys now stretch out further coordinates, same applies for Islands now.

## Why did you make this change?
* Because as I've explained regarding world borders, it's too easy to collide between Island coordinates, and because /is create/restart now stretch out further due to the collide with coordinates issue.
* If we are going to stretch out island coordinates, then might as well stretch Envoy coordinates.

- Finally: Fixed Island coordinates from colliding, rarely, but could still occur.

* Now, it's virtually impossible to have an island collide with a newly created island, because with 0 - 19k, there was hardly a way of colliding new islands and old islands.
* Now, it's like impossible to collide between newly created islands and other islands because from 0 - 500k, it's like impossible to make them the same.
* Essentially like IDS - You can make an ID from 0 to 500k, but they will very unlikely be the same, because of how far it goes.

- Added a brand new VPN Protection system.

- Removed Dead Webhooks that no longer exist.

- Added CrossBow Item to the server

- Fixed island collisions! Yay!

- Upon island creation, it'll now check if an island is already created at that location.

## How does this work?
* Well, thanks to our SkyBlock::class API, we can check if the specific coordinates is at a specific island.
* If it is, it'll return true, and teleport you to another location. If it isn't at an island, it won't teleport you any further. Returns false if not found.

- We've finally added WorldBorders back into the server!

- Fixed block glitching due to coordinates being too far. (No, this full fix hasn't fixed the coordinates issue, but we reduced the coordinates per hand to prevent glitches.)

- Envoy coordinates have been reduced to fix block glitches.

- Fixed crash upon using /changelog.

- Fixed broadcasts with envoys spawnage.

- Added Tip Message to /is kick so it clears up a bit of confusion.

- You can now kick more than one player from your island. Example: Use /is kick iWin10PlayzMC ZeaoPlayzMC to kick the players: iWin10PlayzMC, and ZeaoPlayzMC.

## What is the difference between /is kick and /is remove?

* /is kick - kicks players that are on your island at that time.
* /is remove - removes membership from your island, meaning they won't be able to cooperate with the island, and will be in visitor mode when they next teleport to your island.

- It'll now state if you tried to kick yourself from your own island.

- Improved #💻・console.

- Completely fixed Color coding from appearing on discord.

- Added the following new API Methods:

* Network::removeCode() - Removes the code symbol, including & also.

* Network::getBlockBelow() - Returns the block below your feet, or the highest Y-Value block located at.

* Network::isBlockBelow() - Checks if the block below isn't air.

* Network::sendAlertToStaff() - Sends a alerted message to all staff members available, meaning if they're online.


- Removed the following Player::class methods:
* Player::hasCustomJoin()

* Player::setCustomJoin()

* Player::hasFireworks()

* Player::setFireworks()

* Player::setJoinMessage()

* Player::getJoinMessage()

* Player::getTotalWarns()

* Player::setWarns()

* Player::addKitLevelIncrease()

* Player::removeKitLevelIncrease()

* Player::getKitLevelIncrease()

* Player::getCells()

* Player::getCellByID()

* Player::addCell()

* Player::removeCell()

* Player::loadCells()

* Player::getLastCellSignTapTime()

* Player::setLastCellSignTapTime()

* Player::getLastCellSignTapped()

* Player::setLastCellSignTapped() 

- Renamed the following Player::class Methods:

* Player::getVote(callable $callback) -> Player::getVote(), which now returns an integer.

- We've added a new warning system to this revamp! Before, there either wasn't a warn system, or it needed updating. Now, it'll detect warnings.

## How it works?
* You can use commands like: /warn, and /unwarn.
* Yes, we have made this as simple as possible to make it way less confusing than it was previously.

## New Commands added
* /warn [player] [reason] - Warn another user for the given reason.
* /unwarn [player] - Unwarns another user.

- We've made a ton of changes to how warning works.

## The new system: How it works?
* Well, thanks to our MYSQL Providers, we can use this to make changes, to how it warns, how many warning points it give, etc.
* Currently, the warning points is defaulted to 1 per warn, and can't be edited in any way. This is to prevent major abuse.
* A good thing about our new warning system, is it detects how many warning points you have.
* If the warning points is 3 or above, it'll automatically mute the given player with the reason: "Warned 3+ times", and it'll delete the given warn, so they start over from zero.
* We make this a mute because you really only get warned if it's a chat offense, so this wouldn't make sense if it banned you for something that's not bannable, but rather muteable.
* This makes staff's jobs 10x easier as they wouldn't have to mute the player if they're already muted.
* It'll mute the given player for 6 hours within that reason. If you want to edit that time, you can remute them by using /mute [player] temp [time] [reason]

- We've done a lot of core backends to ensure the server has no issues. This includes:

* Adding Multi-Process support for Player::class loaded subjectives.

## How does Multi-Process core work?
* So it isn't like how it sounds - It's essentially a way to use Multiple Plugin classes, which basically works, when before, it didn't work.

- We've added a new function: Player::getPluginClass() - Returns a main class file, dependant of which plugin used Player::load().

- Fixed crash when using /unmute 

- Fixed crash when using /unwarn.

- Fixed crash when using /unban

- Fixed crash upon loading into the server.

- Added Respawn and Death messages to discord.

- Renamed the following Network::API Methods:

* Network::getStaffMembers() no longer has a parameter of checking the database. It's now restricted via permissions, not rankings.

- Added offline support for the [item] chat messages.

- Added the following API Methods:
* Network::getAdmins() - Get's all admins on the server.

* Network::getManagementMembers() - Returns all staff members that are apart of the Management team. (Including admins).

- Fixed ALERT color coding from not working.

- Added brand new Koth event game!

## How does it works?
* Koth, is an event-type game, bringing this to MCPE (or known as SkyFactions).
* Essentially, the koth game is every 6 hours. 
* Once the koth is opened, everyone that types /koth join, will be teleported to the Koth lobby, where they will wait until the game begins.

## KEEP IN MIND
* Koth game won't start back at 6 hours until the koth game its self begins. This is to prevent conflicts between another round, and the round that is currently there.
* The game starts when there's 4 or more players in the koth lobby, or when somebody uses /koth start.
* We have commands implemented, where you can open the koth lobby, by using /koth prestart.
* This will then open the game to everybody, and those that type /koth join, will be in the waiting lobby.
* Once the game begins, your objective is to be in the capture point AKA THe koth point.
* The koth point, as in where you stand still to receive Capture points. We may call it a name soon, but that's what it'll be for now.
* Once you reach 100 capture points, the game will end, and will give the winning team/solo some rewards. Rewards are currently not added yet. This is the main interface of what koth will be, and how it'll look.
* Though I have finished coding koth, the rewards I haven't yet, which I will push out koth rewards in the upcoming updates.
* If nobody captures the koth in 10 minutes, then nobody will win.

- Fixed /koth bugging out.

- Fixed /koth webhook from not working.

- You can now leave a koth game by using /koth leave (If already in a game or lobby).

- Using /koth join will no longer cause memory fault and fatal errors.

- Using /koth leave will no longer cause memory fault and fatal errors.

- Revamped koth commands to make them better, and respondable.

- Koth Capture points now reset if you're not on the Capture stand.

## Why did you make this change?
* We made this change to prevent any sort of abuse, and making the game easier.

- Fixed crash upon respawn().

- Added support for our Instant respawn system to the Koth.

- Added Boss Bar Support to Koth.

- Fixed crash when sending koth messages to discord.
  
- Fixed Koth timer from starting at 1 second.

- Fixed Game timer for Koth from ending on 1 second.

- Koth game will now always be open, even after server restart. Now, the only time the next koth game can start, is every 6 hours.
* So for example, if the koth game was opened, then there'll be a new saperate timer, which calculates how long the koth has been opened for (Before the koth game fully starts).
* Once the koth game starts, it'll start the event timer to 6 hours. Once the koth game finishes, it'll not be joinable until it's opened again.
* Essentially, this fixes the Koth not being opened upon restarts, when in reality it should've saved it.

- Fixed Boss bar calculations timer.

- All game, pre-game, and lobby timers now start at 0 seconds, instead of 1.

- Fixed capture timer from freezing at an specific capture time if more than one player was in the game.

- Fixed staff chat messages not being sent to discord.

- Added End portal teleportation to your island, at /spawn.

- Upon entering the end portal, you will either be teleported to your island, or if your island hasn't been created yet, it'll automatically create it for you!

- We've finally added NPCS to the spawn (/spawn)

- Yes, yes, and yes! We've finally fixed positions from going to the side of the block when either using /is spawn or using /spawn.

* The fix was because the coordinates had to have .5 at the end of the coordinates, so that way, people could spawn in the middle of the block, rather than on the side of the block.

Thanks to @Bubbly#6984 for bringing this to my attention!

- Fixed hunger drainage when using end portals to go to your island.§
* Though this fix hasn't been fully fixed, it gives you more food hunger health upon teleportation. This seems to fix the issue, for now.
  
- Fixed end portal from not teleporting you for the 2nd time after first entering it.

- Fixed NPC Commands from becoming broken.

- Fixed NPCS from not showing at spawn.

- Fixed NPCS from appearing in different worlds, which shouldn't be shown in.

- Added the following new Player::class methods.
* Player::hasSpawned() - Checks if the user has spawned yet.

* Player::setSpawned() - Sets whether or not they've spawned into the server yet. More preferribly when onJoin() occurrs.

* Player::setRulesRead() - Sets the reading state for the given player. Can be useful for diagnosing whether or not the players have read the rules.
* If they have, it'll set hasPlayedBefore() to true.

- Fixed crash when checking for staff permissions.

- Fixed crash when checking out the rules.

- Added new command: /rules - Checks out the rules for the server, directly in-game!

- Added very good NPC Skins to /spawn.

- Fixed /spawn from teleporting you to an incorrect place.

- Added Info NPC, which shows all the information you need to know about the server.

- Added News NPC, which shows a changelog for the latest version.

- Added Rules to Info Form UI.

- Added Core NPC, which shows all the information you need to know about cores.

- Added basic implementation for Tutorials NPC. Currently, it doesn't work, but we plan to add this in the next update.

- Added Floating Text to spawn, above the end portal, which displays the following:

* How many islands are created on the server.

* How many players are on the skyblock world.

- Fixed bug, where player movement in the skyblock world would teleport you to another location, and can often put you stuck.

- Fixed bug, where when you go to the end portal, it would teleport you to somewhere that's not your island.

- We've now made it so everyone can now delete their own island, by using /is delete.

- Changed prefixes for some faction commands.

- We've modified Player::hasPlayedBefore() a bit, to ensure it supports reading rules, and accepting the terms of service.

- Player::hasPlayedBefore() now only returns true if the player has read the rules. It'll also check for if they haven't played before, but most likely this will return false, as you would need to read the rules and accept the TOS to be marked as "Played before".

- We've added custom erroring system to the rules system.

- We've added checks to ensure the player is new, and if they are, the rules will appear, asking you to agree to the rules, but because of our handy API, we can make it so when you use /rules, this option wouldn't be validated as you're currently playing the server at that time, and wouldn't be able to use /rules if you haven't played before.

- Added /rules - This command will allow you to read the rules without the acceptance mark.

- Database should now go offline instantly. It'll check for its playability, to check if the database is still down, or online upon next database refresh.
* Currently, this works for both offline and online gameplay.
* This means there should be less issues with database crashes because the database goes offline before it communicates with the server.
* The reason why we have the database refresh (every 60 seconds), is so it can check if the database is active/inactive or even offline. Because it only deactivates instantly when the database goes offline. This is to prevent crashes to the server because of database issues.
- Fixed crashes when database goes back online, then goes down, it'll crash the server.
* Because of the database update above, databases will deactivate instantly, dependant on whether or not the database is active.

- Fixed crash when envoys automatically despawn if you're on the server.
* This was because of poor checks to ensure the envoys have either despawned or not.

- I've completely modified Player::teleport(), to ensure spawnpoints with center blocks are fixed.
* We've also added a parmeter, where you can check if the position should be re-positioned to 0.5 x and z. If yes, it'll attempt to find X and Z's 0.5 (Center blocks) positioned.

- We've added the following Player::class methods:
* Player::positionSpawn() - Re-positions the given coordinates, depending on the coordinates given in the parmeter(s).

* Player::getSpawnLocation() - Returns the given spawn point. The reason why we've added it to Player::class is simply because of backwards compatibility, and to ensure we can use spawn locations in classes that actually matter.

* Player::setSpawnLocation() - Sets the spawn location at the exact coordinates the player is at.

** To put it simply, setSpawnLocation() also repositions the spawn point the player is standing at.

- Fixed spawning on the edge of the block for all locations that use Player::teleport() method.

- Fixed special character issues with /rules, and /changelog.

- We've re-coded a few skyblock commands to ensure it's better than ever.

- Added the following new SkyBlock Commands:
* /is invite - Invites another player to your island.

* /is accept - Accepts a player's island invitation.

* /is deny - Denies a player's island invitation.

- Removed the following SkyBlock Commands:
* /is add

- We've saperated /is visit, replaced it with /is home, and made /is visit a saperate command.

- /is visit will now bring a UI, where you can teleport to a player's island.
* This is so much easier than using commands to teleport to a player's island.
* /is tp will be for your own island, whereas /is visit will be for teleporting to other player's islands.

- Fixed /is accept from not sending the join message to all island members.

- We've now sorted the player names alphabetically from /is visit UI.

- We've added how much total islands have been created from the Visit UI.

- You can no longer invite yourself to your island.

- You can no longer accept yourself from your own island.

- You can no longer deny yourself from your own island.

- Completely re-coded Command mapping for SkyBlock plugin, cleaning plugin.yml, and allowing the server to load commands better, and more reliable.

- Along with this change, we've removed permissions from plugin.yml, and made our own Command map system. A bit like PMMP, but our very own! With a useful getCommands() array, to fetch all the skyblock commands into one, clean code.

- We've finally added Form UI's to the /is command.

* We've actually made it so you can use either forms, or commands. To use forms, just type /is help, /is, or /is test (an example of a invalid command).

- We've added a lot of icons to SkyBlock Forms.

- Fixed a lot of argument errors.

- All usages now come under getUsage() when typing a usage out, instead of the per-usage system.

- Added a new class: SkyBlock::getCommandMap() - Where all the command mapping takes place!, alongside registeration, unregisteration, etc.

- Fixed crash when clicking the X button on Custom Form UI's that have the input option.

- Fixed /is kick from incorrectly kicking users.

- Fixed Visit menu from not bringing you back to the menu if you close out of the Visiting menu, and if you previously went to that menu whilst in the main skyblock menu.

- Admin commands no longer display in /is help UI if you don't have permission to them.

- Mark the user has permission if the permission node is null.
* This means we can use hasPermission() in all of our commands. We don't have to, but we can now if we want to.

- Fixed end portal from not teleporting you to your island.

- Island's help UI is now in alphabetical order.

- Added Home commands!

- Added /home set
- Added /home tp
- Added /home list
- Added /home delete

- We've changed Combat tagging, and how it works.
* Changed Combat timer to 15 seconds.

- Use CombatTag's new API methoding to ensure the user is combat tagged before sending them the timeout message.

- Fixed /home delete command from not displaying the home name correctly that you wanted to delete.

- Fixed heads duplicating upon death().

- Fixed death messages duplicating upon death.

- Fixed world conflictions.

- Fixed not being able to move after you've read the rules.

- Removed Instant respawn system as that became buggy.

- Fixed crash when closing the /rules UI, by clicking Submit. This was because of the rules acceptance, which won't show if you've played before.

- Fixed being able to bypass the Visiting system.

- Added a new parmeter to Player::teleport(): $levelSupport.
* If $levelSupport is true, it'll provide true level support, for example, if you're teleporting to another world, then this option would be useful for that.
* If $levelSupport is false, it'll teleport to the coordinates that are in the current world you're in.
