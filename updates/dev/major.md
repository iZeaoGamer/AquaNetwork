## VirtualPE Development updates:

## This changelog introduces a new and complete Core revamp, along with: Major API changes (API BC), and many changes with the concurrent server.

- Start work on SkyFactions (Our first mixed gamemode), between Factions and SkyBlock.
- Added a very unique way of raiding: Cores. (Info at #👀・spoilers.)

## What are Cores?
- Cores, are essentially a way of raiding. If you have a core, then you can't be raided. If your core get's destroyed, raiding is possible. Try to protect the core as much as possible, fight enemies, and get them away from the core.


## How does a core work?

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

## How they work?
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
- ## Removed the following API Methods:
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

- ## Renamed the following API Methods:
* Network::number_format_short() -> Network::shortNumber(), and improved the function.
* Network::calctime() -> Network::getFullTime()
* Network::timeFormat() -> Network::getFullTime()
* Network::timeToSeconds() -> Network::getFullTime()
* Network::isLobby() -> Network::isLobby() - Returns bool instead of string.

- ## Addded the following new API Methods:
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

- ## Added the following new API Methods:

* Network::removeCode() - Removes the code symbol, including & also.

* Network::getBlockBelow() - Returns the block below your feet, or the highest Y-Value block located at.

* Network::isBlockBelow() - Checks if the block below isn't air.

* Network::sendAlertToStaff() - Sends a alerted message to all staff members available, meaning if they're online.


- ## Removed the following Player::class methods:
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

- ## Renamed the following Player::class Methods:

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

- ## Renamed the following Network::API Methods:

* Network::getStaffMembers() no longer has a parameter of checking the database. It's now restricted via permissions, not rankings.

- Added offline support for the [item] chat messages.

- ## Added the following API Methods:
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

- ## Added the following new Player::class methods.
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

- ## We've added the following Player::class methods:
* Player::positionSpawn() - Re-positions the given coordinates, depending on the coordinates given in the parmeter(s).

* Player::getSpawnLocation() - Returns the given spawn point. The reason why we've added it to Player::class is simply because of backwards compatibility, and to ensure we can use spawn locations in classes that actually matter.

* Player::setSpawnLocation() - Sets the spawn location at the exact coordinates the player is at.

** To put it simply, setSpawnLocation() also repositions the spawn point the player is standing at.

- Fixed spawning on the edge of the block for all locations that use Player::teleport() method.

- Fixed special character issues with /rules, and /changelog.

- We've re-coded a few skyblock commands to ensure it's better than ever.

- ## Added the following new SkyBlock Commands:
* /is invite - Invites another player to your island.

* /is accept - Accepts a player's island invitation.

* /is deny - Denies a player's island invitation.

- ## Removed the following SkyBlock Commands:
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

- You can now fit /is desc all in one text upon going towards someone's claim.§
* Because we use wordwrap(), this is actually possible. Every 15 width, a new line will occur in the string/message.

- We've added back Instant respawn, but more basic.

- Fixed crash when hitting the ground too hard message attempts to occur.
* This was because we didn't implement this type of message ourselves. My mistake!

- Fixed dying multiple times in a row.
* This issue was because of the respawn timer. This caused issues with the server, so we therefore recoded it.

- Upon death, it'll now automatically teleport you to spawn.

- Upon death, it'll now also activate PlayerRespawnEvent() for further support compatibility.

- Fixed lag upon death(), and upon pvp().

- Fixed dying in protected areas, if you fell from a high place.
* This was because we weren't checking if the EntityDamageEvent() was cancelled, and didn't add the @priority tag as Monitor.

- You can no longer die if you're in /fly.

- You can no longer die if you're in creative.

- Fixed /rules from appearing as the color symbol at the end of the whole rule book message.

- Added support for in-game rules only in /rules. To view rules on our discord server, you can read them there!

- Added Discord link to /rules.

- Fixed death messages from occurring twice.

- Fixed crash upon leaving the game after /is create was executed.

- Fixed crash upon leaving the game after /is restart was executed.

- It'll now only create your island if you don't log out during the /is create process. If you log out, the island creation will cancel.

- It'll now only restart your island if you don't log out during the /is restart process. If you log out, the island recreation will cancel.

- Fixed /is create from removing all of the island datas.

- Fixed /is delete from removing all of the island datas.

- Fixed /is restart from removing all of the island datas.

- Plugin loading discord message is now in alphabetical order.

- Plugin disabling discord message is now in alphabetical order.

- Fixed Koth Webhook.

- /is visit will now display "No islands created" if no islands have been found.

- Fixed island corruption crashing the server.
* If for some reason, a user's island data was corrupted, it'd crash the server. Now, it'll give you an error regarding this, and to contact support. (Like using commands that relate to your island).

- /idle now broadcasts it into the console channel on discord.

- Revamped /is top.

- /is top now supports multiple pages.

- Updated /is top UI, and added support for multiple pages.

- You can no longer add unlimited pages to /is top that are empty.

- Fixed /tp from teleporting you to an inaccurate coordinates, or the player's coordinates, but inaccurately.

- Fixed /spectate on <player> from teleporting you to an inaccurate player's coordinates.

- Fixed Online TP, or selecting a player UI to teleport to, from teleporting you to an inaccurate player's coordinates.

- Fixed /tp from not teleporting you to the coordinates.

- We've removed the Factions plugin, and made support for SkyBlock only, in terms with commands. Yes, this is still SkyFactions, but having two plugins are a bit confusing, and just isn't needed. You can play SkyFactions than you'd normally would, just removed the plugin its self, as most of the commands we're not even using due to the server's concept, and us already implementing most of the features.

- ## Added the following new commands:
* /is guardian - Spawns a guardian to protect your island.
* /is shop - Opens the Island shop.

- Removed Faction map from scoreboard, as that didn't actually work for some reason.

- Made ActivityPoints via the database, instead of a .yml file.

- Scoreboard is now a lot smaller than previously.

- Fixed crash when using /is shop.

- Fixed crash when using /is guardian.

- Fixed crash when trying to obtain Banknotes from /is shop.

- ## Added the following new API Methods:
* SkyBlock::getIslandRank() - Returns a island ranking, as apart of /is top.
* SkyBlock::getGuardians() - Shows how much guardians you currently have. Returns integer.
* SkyBlock::setGuardians() - Sets the amount of guardians you currently have. Most preferably how much has spawned.
* SkyBlock::sendTopIslands() - Sends the top 10 most valued islands along with the page specified by the sender.
* Player::getActivityPoints() - Returns how much ActivityPoints you have.
* Player::addActivityPoints() - Adds the given activity point to the player.
* Player::removeActivityPoints() - Removes the given Activity point to the player.

- Fixed color coding issue with obtaining the player name that had their core destroyed.

- Fixed issue, where falling into the void will always set your state to Visitor. Now, this shouldn't occur.

- Fixed being able to obtain unlimited starter items, by using /is create or /is restart, constantly lot out, and log back in. You do the same process over again, and you would then get unlimited items. Now, this has been patched.

- Fixed Guardians amount from going into the negatives. This is because iron golems take longer to die from the void (Due to their health being at 100 HP), and therefore, takes away the amount of guardians, used as negative numbers. This has since been patched.

- We've now renamed the Island per name in /is top to their actual island name, instead of the player's name.

- We've added a new argument: <name> for both /is create and /is restart. This is because we're relying on island names now, instead of player names.

- Renamed command: /is name -> /is rename.

- Upon going into the end portal, it'll now ask you what name you'd like your island to be. If you close out, and you move, it'll open again, and so on.

- /is create and /is restart with no more arguments will now open a Form UI. We may do this with most commands in the future.

- We've changed /is help UI, so it shows the usages now, instead of only the command names.

- ## Added the following new API Methods:
* SkyBlock::getIslandByName() - Returns only the Island that has a name.
* SkyBlock::isSameName() - Returns if the island name given is the same as any of the island names found. Returns true if the same, returns false if not the same. 

- ## Renamed the following API Methods:
* SkyBlock::getIslandName() now returns island leader/member prefix alongside the island name(s).
* SkyBlock::getIslandRank() now returns null if the island/island name isn't found.

- You can no longer (re)name a already-existing island.

- We've completely changed how SkyBlock Chat formatting works.

## How does the new chat formatting work?
* We've made many changes on how chat formatting works. Essentially, we now have Island member/leader prefixes. If you're a member of a island, it'll state * before the island name. If you're a leader of an island, it'll state ** before the island name.
* We've also added Island ranking chat to the server. It's basically faction rank, but island ranking. It'll state what place you are in /is top, so say if I was 3rd top island, it'll state "#3" with the island prefix and island name.
* We've added these implementations because I wanted to be one of the first MCPE Servers that provided faction-like ranking formatting, as described here.
* Yes, we do have it differently than any other servers. Island ranking works with /is top, allowing you to know what place someone is in /is top, directly in chat. This just makes it 10x better than it was previously.

- Fixed Island claim displays from displaying the island member/leader prefix.

- Fixed Island description display when entering a claim from not cutting the long-ass word, if it's one word, but really long.
* Before, it wouldn't make a new line if the long word is at the width limit. Now, it'll make a new line.

- Changed /is help UI, to make the color coding a bit more unique and better.

- Fixed cooldown on minions when leveling up.

- Fixed crash when leveling up the Mage minion.

- Fixed crash upon spawning an automatic island guardian, using Mage Minion.

- Fixed Nametag above player's head.

- Added more Devices display support to the Scoretag/Nametag.

- Blocked people being able to use /tp whilst in visitor mode.

- Blocked people being able to use /spectate whilst in visitor mode.

- Fixed being able to execute /spawn more than once, which would lead to it becoming buggy, having more than one timer enabled at once.

- Fixed crash when giving yourself an id that is out of bounds. Now, it'll default it to stone when you exceed the ID packet limit.
  
- Item names now need to be valid, instead of causing you to crash.

- Fixed all client crashes, and player data corruption when using /item incorrectly, such as when you're giving yourself the id: 1000000000000000000, when that's not an id, and that causes to crash because it's out of reach.

- Removed /give, and replaced this with /item.

- Added randomised spawn countdown timers (From 1 - 15 seconds).

- Added Kills and KillStreaks to the server!

- Added multiple /is top types support to the server.

- Added /is top kills

- Added /is top killstreak

- Fixed Minions from not despawning properly.

- Updated /is top UI to display island values.

- Added Kills and Kill Streaks to the scoreboard, which was proprosed by the suggestion: #61.

- Added /is addstate (For management only)

- Added new command: /is info - This command will allow you to check for either your or other player's island information.

- Added Island Info to Island Management UI.

- Updated /is top UI, and add support for multiple types.

- Updated server to the new Minecraft Version: v1.17.0.

- Fixed crash upon joining the server.

- Fixed crash when setting a game rules changed packet.

- Added Ding sound when hitting another player using a bow.

- It'll now display information on the given player when hit by an arrow.

- Elytras now function, like in Vanilla.

- Locking your island will now automatically teleport those that are a visitor to spawn, as per requested.

- Fixed crash when using /is lock.

- Added Island value, and Island ranking to /is info.

- Island ranking will now display for all island roles, and not just leader.

- Added new Core upgrade: Regenerate Core Health. This upgrade, will allow you to heal your core, within a specific amount of seconds. This uses Regeneration effect, and you can buy Regeneration effect for your core from Level I - IV, which lasts for 10 seconds before the upgrade is gone.

- You can no longer hit yourself using a projectile.

- Changed the error message for Hitting yourself using a projectile.

- Renamed command: /upgrade -> /is upgrade.

- Added /is upgrade UI to /is Management UI.

- Fixed taking damage from lava or fire when you're in visitor mode.

- Fixed crash when using /ban.

- Fixed crash when using /warn.

- Fixed crash when using /mute.

- Fixed crash when using /unban.

- Fixed crash when using /unwarn.

- Fixed crash when using /unmute.

- Fixed crash when obtaining a tag.

- Fixed crash when the tag does not exist.

- Fixed crash when obtaining a tag note.

- Added vanilla command autofill system.

- Added new command field: /ban [player] list.

- Added new command field: /mute [player] list.

- Fixed server crash when deleting your island.

- Fixed server crash when island name is null.

- You can no longer join more than one island.

- There is now no arguments to /is leave, as that'll count towards the island you're a member of.
* Now, it'll check for the leader of the island you're a member of. If it appears you are the leader of the island, it'll state "You can't leave your own island". If you're not apart of any islands, then an error message will appear.

- We've completely re-done some parts of the Island UI interface.

- We've removed the following /is commands:
* /is on
* /is members
* /is rank
* /is value

- Most of the island commands removed, are because /is info already has them, so no need to duplicate the messages.

- We've re-categorized a lot of island UI Commands. Here's what's been recatgorized:
* /is top: Island Management -> Island Profile
* /is info: Island Management -> Island Profile
* /is help: Main UI -> Island Profile
* /is visit: Main UI -> Island Profile
* /is leave: Island Management -> Island Profile

- We've added the following new sections in /is info:
* Is Leader - Checks if the player name you entered from /is info, is the leader of the island.
* Banned Players
* Leader Online
* Visiting an island: Keep in mind - This section will only appear if the island leader is online.

- We've renamed the following sections in /is info:
* Island Ranking: Now has a # before the ranking position.

- We've made some changes with /is visit.

- Island names will now appear next to the leader's name from /is visit.
* This will make things 10x easier, so you don't have to go looking at the island name that the player is in.

- AFK Pools will no longer stop you from being A.F.K or Idle. Instead, it'll still afk or idle you, no matter what.

- ActivityPoints will no longer continue if you're in AFK or Idle Mode.

- Fixed crash when you sometimes try to join the server.

- Renamed main command: /is teleport -> /is home

- /is home will now teleport to your leader's island, instead of only teleporting to your island if you're the leader. For example:
* If you weren't the leader of the island you're a member at, /is tp wouldn't work, and simply wouldn't teleport to your leader's island.
* Now, /is tp will check for your island's leader name, and will then teleport to their island. If the leader name isn't found, an error will appear.

- /is leave will now teleport you to spawn. This is to prevent abusing a bug/glitch with being on the player's island whilst you type /is leave.

- /is create can only be executed if you're not apart of any other islands.

- Changed some moderation behaviors to ensure the server is at a better moderation status.

- Fixed /is ban from incorrectly banning a user from your island.

- Changed all island leader related errors; If the user isn't the leader, or not in an island, then it'll now state this.

- Added new section to /is info: Island Rank Name/Symbol.

- You can now use /is info on other players freely when you aren't in an island. Before, an error would occur.

- Added the following new island commands:
* /is chat - Toggles on/off island chatting.
* /is here - Checks what island you're standing on.

- We've changed the following alias/commands to their new commands:
* /is disband - Deletes an island.
* /is home - Teleports you to your island home.
* /is sethome - Sets your island home.

- We've added the following island aliases for commands:
* /is create: /is make.
* /is description: /is motd
* /is disband: /is delete
* /is guardian: /is protector.
* /is help: /is ?
* /is home: /is tp, /is teleport, /is spawn
* /is private: /is lock.
* /is sethome: /is setspawn
* /is top: /is leaderboard, /is lb

- Fixed double spacing in Player tags.

- Fixed crash when using /is remove.

- Fixed Player's nametag above from always appearing with the leader symbol, even if they're not actually the leader.

- The server will now broadcast when your island member joins the game.

- The server will now broadcast when your island member leaves the game.

- Added the following API Methods to SkyBlock::class:
* SkyBlock::isMember() - Returns true if it's a member of this island, returns false if you're not.
* SkyBlock::isLeader() - Checks if you're the leader of an island. Returns true if you are, returns false if you are not.
* SkyBlock::isMemberSymbol() - Checks if you have the member symbol (*). Returns true if you have, returns false if not.
* SkyBlock::isLeaderSymbol() - Checks if you have the leader symbol (**). Returns true if you have, returns false if not.
* SkyBlock::getIslandSymbol() - Returns the string symbol (Either ** or *), or "..." if not found.

- We've completely re-coded /is commands, and the commands and its messages are now form based UI's.

- Fixed crash when using /is delete

- Fixed crash when using /is restart

- It'll now state if the creation type is "created", or "restarted".

- /is kick can only kick one user per command, not multiple. This was apart of the new /is UI update.

- Added Island Chat to Island Profile UI.

- Added Island Here to Island Profile UI

- Added Island Protector/Guardian to Island Management UI.

- Added Island Shop to Island Profile UI.

- Fixed booleans returning 1 as a display message in certain commands/Island UI's.

- Fixed /is restart from sometimes allowing the core to fall into the void.

  - Fixed miner minion from despawning upon every restart.

- Fixed multiple cores from spawning at the same time.

- We've completely re-done Island generation, and how it works.

- There is now a queue for creating/restarting your island.

- Added a new queueing system to the server.
**How it works?**
* When you join the server, you will be added to the queue alongside your queue position spot.
* The more the players, the longer the queue time is and queue position spot.
* NOTE - Ranked players and Staff will be in the higher priority queue list.

- Added a new Anti-Glitch system to the server.
**How it works?**
* We have a new system implemented now, that disallows the following:

- Breaking protected blocks

- Placing protected blocks

- Ender Pearling phasing.

- The anti-glitch implementations for Break and placing will now teleport you to prevent going through blocks. That's how our anti-glitch system works.

- Fixed issue when cancelling EntityTP() it would crash the server.

- You can no longer use /is sb if you aren't in an island.

- Deleting your island will now disable Island scoreboards. That way, it'll prevent server crashes to do with islands not being found.

- Completely revamped our Moderation system completely. Here's what we've changed:

- Removed the following commands in flavour of /moderate:
* /vanish
* /reveal

- Our moderation system now has a built-in disguise system.

- We now have a paid hosting service! Thanks to @Tivercey for buying the server for us!

- We've completely re-designed our scoreboards system.

- Every scoreboard type, will have a different design-color, which makes it unique from everything else.

- Added a new command: /hud.

* This command, will allow you to open the scoreboard editor. In that UI, you can choose which scoreboards you'd like to enable/disable.

**KEEP IN MIND**

* You can only enable one scoreboard at a time.

- We've added a brand new spawn! Still not finished yet, but massive thanks to @Bubbly, and a bit of thanks to @Tivercey for helping out with the spawn!

- We've added Always Sunrise time.

**How this works?**

* In the new spawn world, it'll be stuck in Sunrise time. It makes the feeling good as well! :)

- Added Support for Minecraft: 1.17.10.

- Added the following new channels to discord:
* #staff-movement
* #public-support
* #private-support
* #report-details
* #staff-reports
* #public-reports
* #response-time

- Removed the following channels on discord:

* #staff-support -> #private-support
* bug-report -> #public-reports
* staff-report -> #public-reports
* player-reports -> #public-reports
* #punish-format
* #the-global-protocol

- We're now supporting MySQL Offline databases.

**How it works?**

* So basically, we support most of the features whilst the database goes offline. If it goes offline, all of the data will automatically be set as a SQLite database, until MySQL comes back online.

- We've changed our setting a player's rank command usage.

- We've added discord support for /setgroup.

- We've completely re-designed our Ban, and mute system, to make it mobile friendly.

- We've renamed the discord channel from #sneakpeeks -> #spoilers to prevent spelling confusions.

- Fixed Island Scoreboard from becoming too large.

- Fixed crash when you don't have an island, and you try to turn the scoreboard on.
* Although, it'll say you turned it on, there are now checks added, where it'll check if you have an island. If you don't, the scoreboard will not display.

- Fixed Floating Texts from lagging the server.

- Added the following leaderboards to PvP Area:
* Island Value Top
* Richest player top. (Money)
* Kills
* Kill Streaks
* Most active players 

- Added a brand new spawn! Big thanks to @bubbly for building it!

- Moved NPCS to the new spawn.

- Staff can no longer break/place blocks in Regioned areas, unless they have build mode on.
* Now, this had came as an issue for some time now.
* Basically, this means those that were protected using worldguard,
* will now not allow staff or anybody from breaking/placing blocks unless they use /buildmode on.

- We've added a little hot/house for the Queued players.

- We've re-done a bit of the Queue system.

**What's been changed in regards to our Queuing system?**

- Added Floating Texts to queued players.
* Essentially, when you're in the queue, the floating text will appear infront of you.

- The queue timer is much shorter than previously.

- We've added Estimate Wait Time to Queue FT.

- And that was about it with the Queue changes.

**Server-Side Changes**
- Fixed PvP being turned on at spawn.

- Added PvP Arena.

- Added a huge koth arena! Thanks to bubbly for helping with the areas that needed filling.

**Feature Changes**

- Removed Trojans entities. They'll now act like invisible entity. Let me explain to you how it will work:
* Trojans do not display. Every so minutes, the trojan will go onto a random user's island, and if they have a minion, depending on the chance, it'll remove a random item from the minion inventory.
* But that doesn't end there. You can still use your perks/upgrades from the minion's upgrade system to protect the minions from trojans attacks.

- Added unstabled Races. We will improve on this overtime, but currently, it may be unavailable for use.

**Server-Build changes**
- Added Welcome floating text messages.

- Added PvP Floating text to the PvP Area hole, which takes you to our PvP Arena.

- Fixed duplication of Island Value Top title, which before, appeared twice.

- Removed "Data refreshes every x seconds" at the bottom of each leaderboard.

**NetworkCore V2.0-dev Version**
- We've completely re-designed our Network Core's namespaces.

- All API related methods will go in \core\utils

- All namespaces are now built with: core\, instead of VMPE\Zeao

- We've replaced GalacticPlayer Class with: CustomPlayer Class.

- Our Player class namespace is now built with: \core\player, as pre-described in api 4.0, which is what will happen in api 4.0.

- Replaced core\Discord\Zeao to core\discord

- Replaced core\Ranks\Zeao to core\ranks

- Replaced core\ to core\bossbar

- Moved all of the commands to core\commands

- Remove core\essential, and make them all in core\commands

- Removed duplicated core\event(s) folders.

- Fixed a recent bug, where if you try to turn off vanish, even if you're not vanished, it'll say "You have been vanished for 5 decades".

- Fixed envoys from lagging the server.

- Fixed our anti-glitch system from glitching you inside a block, which allows you to block glitch.

- Added /is customspawn
* This command will allow you to create a custom island spawnpoint.
* Note - THose management, do not use this! It could mess up with the current layout/setup. Thank you!

- As of NetworkCore v2.0.0, we've now added "Traits" API.

**What is a trait?**
* It's a type of class where you can add a use case after the class code, which allows you to use API Methods in the given trait that you've enter, which would work for Network class, as an example.

- We've moved everything non-network related subjects to its own respectful trait.
* In the upcoming future (Hopefully by api 4.0.0), we will be moving everything that doesn't involve around Networking to its own respectful class.

- Fixed envoys from completely breaking the server.

- Fixed envoys timers from going back to 60 minutes, which should've expired, and not reset back to the given counter, unless a new one spawns.

- Fixed fireworks from only appearing once.

- Fixed chest from constantly appearing back whenever you tried claiming the envoy reward.

- Added new command: /shop.

- Fixed issue with ores - For some reason, I made it as oreos, not ores. Sorry!

- We've finally fixed all Shop icons from /shop!

- Moved floating texts at spawn to each corner. Thanks to @Bubbly for this suggestion!

- Fixed an issue where you were unable to eat in the PvP Arena.

- Fixed an issue where you'd lose your hunger in PvP Arena!

- Fixed an issue where you'd take fall damage upon entering the arena.

- Fixed issue with PvP Arena End portal from not teleporting you to the arena, but instead, it would teleport you to your island/create an island UI.

- Fixed loading in data from keeping you as a queued player.

- You can no longer fly in the PvP Arena. (If you aren't staff.)

**NOTE**
Staff will need to be in vanish to not have their fly disabled for security reasons. They aren't allowed to abuse their power on it or they would be demoted.

- Added KDR Leaderboard to PvP Area.

- Added Personal Stats at spawn.

- Fixed KDR Leaderboard.

- Fixed Kill Streaks Leaderboard.

- Fixed block drops from becoming broken, and nothing would drop.
* This was because of the gamerule: doTileDrops, which was set to 0 AKA false.

- Time set is now always mid day for the following worlds:
* PvP Arena
* Koth Arena.
* The queue world.

- Fixed kill streaks/kdr ranked numbers from appearing incorrect top stats.

- Fixed ranking position of kill streaks from being incorrect at Spawn, personal stats.

- Rename type from streaks to streak as that was what it was set to in the database.

- We've added our own Enchantment Shop UI, where you can buy vanilla enchants!

**How it works?**
* So you type /shop, go to "Enchantment Shop", and then click on a enchant category. Once you've selected one, you can buy an enchant within that category.
* After selecting, it'll confirm to you if you're sure you want to buy this enchant. Click "Yes", and it'll state if you've bought it or not.

**A good thing about this feature**
* We have an automatic upgrade system to the Enchant shop. Already got sharpness level 1? When you buy it again, it'll state you've upgraded the item to Sharpness level 2.

- We've reverted the startup() messages to our old, but better startup system for the Network core.
* Essentially, this means startup() is 10x faster than before. Say good bye to the previous startup() system, and say hello to our fastest system we currently have in place.

- It now only takes a few seconds for the startup() to fully enable everything. Before, it would take from 30 seconds to a minute or two just for it to start up, which is really long for a server.

- Gold ores now drop Gold ingots.

- Iron Ores now drop Iron Ingots.

- You can no longer hit people that are coming down to PvP Arena.
* This means, if you and someone else both warps at the same time, you both can't hit each other until you're near towards the ground.

- You can now use ender pearls whilst in the PvP Arena.

- Flying whilst in the PvP Arena now relies on whether or not the user is vanished, rather than with staff permissions.
* We've done it this way for security reasons.

- You no longer take fall damage in Koth Arena.

- Moved the following to /shop:
* Island Shop
* Fuel Shop
* MotherBoard shop

- Removed the following commands:
* /is shop -> /shop.
* /is sb -> /hud 
* /fuel
* /is netherspawn -> moving this to Island /setspawn command.
* /is netherzone -> Moving this to island /setzone command.

- Fixed crash when confirming your purchase with money!

- Fixed incorrect amounts of currency being used.

- Fixed players not being able to hit you if you turned on build mode for the current session.

- Completely re-designed MotherBoard Shop.

- Renamed everything in the MotherBoard shop from Core -> MotherBoard Shop.

- You can now spawn a new motherboard, by buying it in the core shop.

- Fixed Currency Converter from converting incorrectly.

- Added a lot of new Island Admin commands to Island Admin panel.

- Added the following new Island admin commands to the Admin panel UI:
* Custom Spawn
* Create World
* Reload Data.
* Set Zone
* Set World
* UpdateZone

- You'll now get teleported to the queue area upon spawning into the server, instead of when you actually have spawned.
* This is because onJoin() wouldn't activate teleportation instantly. Instead, it would stay where you are for a few moments before teleportation.

- We've revamped our discord server entirely. Removed a lot of channels that weren't needed, and made the discord server cleaner.

* Here are the following discord channels that are being removed:
- #😡・staff-reports -> #💼・management
- #👥・staff-list -> #ℹ・staff-info
- #ℹ・punish-info -> #📳・moderate
- #🤬・warn-words -> #📳・moderate
- #💻・console -> #🎑・minecraft
- #👊・punishments -> #📳・moderate.
- #🏠・build-reference
- #🔨・build-plans -> #📝・server-ideas.
- #📀・db-status -> #🎑・minecraft.
- #💻・response-time -> #🎑・minecraft.
- #🐱・tyler’s-ideas -> #📝・server-ideas.
- #🛑・reports-details -> #📳・moderate.
- #👀・staff-activity -> #🎑・minecraft.
- #👋・inactive -> #👋・inactive (May change this if I make this more of a purpose.
- #🤞・staff-movement
- #📸・media -> #💬・global 
- #🙋・support -> #👥・public-support or #🤫・private-support.
- #👥・team-members
- #💭・discuss-talk 
- #🌛・apply-here -> #📢・newsletter
- #🎊・updates
- #🔈・voice-rules -> #⚠・global-rules 

**Staff Categories**
We've (for the last time now), reorganised the categories.
Meet our following staff categories:

**Server Wide (STAFF)**
This channel is where staff information and news letters are announced.
Here are the channels that is in this category:
#📣・staff-news
#ℹ・staff-info

**STAFF TEAM CHATS**
This is where all staff chat related goes.
Here are the channels that are in this category:
#💬・staff-chat
#🕴・higherups-chat.

**Staff Team Voice**
This is where all of our staff voice calls take place!

**Staff**
Here is where everything takes place. Console logging, server suggesting/ideas, Moderation, Punishment logs, and more!

**Here are the channels that are in this category:**
#📳・moderate
#📝・punish-logs 
#💼・management (For management only to see).
#🎑・minecraft (For things that happen in-game!)
#📝・server-ideas

**STAFF MISCELLANEOUS**
This is where the other channels that didn't quite fit the category names belong to.
Here are the following channels that are in this chat:
#👋・inactive
#🎉・promo-demo 
#🚨・to-do
#📝・modlog 
#🤖・staff-cmds 
#🤡・exposed.

**PUBLIC CATEGORIES**
This discord revamp includes a few categories changes, making the discord server more organized.

Here are the following categories and for which channel:

**SERVER DETAILS**
This category will help with finding the server information you need to join it.
These are the following channels in this category:
Server IP
Server Port
Vote Link
Release Date (Remove soon)
Store

**Server INFO**
We've done some changes in relations to this.
These are the following channels in this category:
#🚀・booster
#❓・faq
#👋・user-state 
#✅・verification 
#👥・partners

**SERVER WIDE**
This category is where all of the server network related content is published. So like news, rules, and things that make your game experience better, that is, if you like spoilers.

Here are the following channels in this category:
#📢・newsletter
#⚠・global-rules 
#👀・spoilers
#🎉・giveaway 
#🗳・polls
#📝・change-log 

**SERVER ROLES**
This channel is where you go to verify your roles.
Here are the following channels in this category:
#☀・self-roles
#🌈・color-roles

**Social**
This is where you become social. Interact with our community, chat with the staff, and making friends.
Here are the following channels that are in this category:
#general -> #💬・global
#🤖・bot-cmds
#👍・suggestions 
 
 - We've added MotherBoard rewards.

 **How it works?**
 * When you raid a motherboard, the person that raided it can receive rewards. Rewards are in the Info UI in Motherboard section.

- Fixed crash when using TNT to explode blocks.

- Fixed issue when exploding, items dropped will be duplicated.

- Fixed being able to use flint and steel in protected areas.

- Added Clear Lag to the server.

- Clear lag now clears items once every 10 minutes.

- Fixed Queue floating texts from not disappearing after you've entered the server via our queue system.

- Fixed Queue floating texts from appearing in the same coordinates in all worlds.

- A raiding sound will now occur if a player that isn't apart of your island, and that isn't visitor, attempts to go to your island.
* Though, there had been spoilers of a raiding sound occurring, but at that stage, it was only when you use the raiding minion to raid the base. Now, it'll do it every time someone finds your island.
* The raiding alert will occur once every 10 seconds to prevent title spamming.

- Added the following new island commands:
* /is Fly
* /is find
  
**/is fly**
- Allows you to fly on your island. Cannot be used if you aren't in an island, or if you're flying in an island you're not apart of.

**/is find**
- It's basically /is map (/f map), but because we're unique, I've decided to completely rename the system to /is find.

- Your fly will no longer disable if you have bought fuel, and if you are under a block, basically the Highest Y Coordinate at your location, and whether or not it's a block, it won't disable your fly.

- You can now fly freely on islands you're apart of.

- Fixed envoy platforms from not disappearing after 10 seconds.

- Fixed spawners floating text from appearing incorrect information if there are more than one person viewing the floating text.

- You can no longer place minions in areas that you shouldn't spawn them in.

- Fixed crash when claiming envoys.

- Fixed crash when flying sometimes.

- Added /is ally command.
* This command allows you to ally with other island leaders.
* Allying also allows you to teleport to their island, even if it's locked.

- Added the following Ally commands:
* /is ally list - Shows a list of your allies.
* /is ally add <leader> - Sends an ally request to another island leader.
* /is ally remove <leader> - Removes an ally from your island.
* /is ally accept <requester> - Accepts an ally invitation request.
* /is ally deny <requester> - Denies an ally invitiation requet.

- Fixed allying from not actually allying you.

- Fixed Allying duplicate, where it'll say an island's name twice, or it just won't add the island, only one of them.

- Fixed allying from resetting your data.

- Added **BRAND NEW** CRATES to the server!

- Chances can now be float chances in Crates and Envoys.

- We've added our very own custom Menu for Opening a crate.

- You can now get Sky keys from envoys.

- Added more things to Market, big thanks to @Bubbly for doing that!

- You can now use a brewing stand to open the AuctionHouse.

- You can now use a Shulker box to open the /shop UI.

- Added Crates area to Spawn.

- Added Auction House area to Spawn.

- Added Server Shop to Spawn.

- Added Obsidian Breaker.

**HOW IT WORKS?**
* So Obsidian will have health.
* Essentially, the total health of Obsidian is 10.
* You can destroy its health per explosion using TNT.
* Once there is no more health, the obsidian block will break.

- Moved Raiding related items to a new shop category: Raiding Category.

- Fixed MotherBoards from being able to be put in the void.
* This was an issue for some time now.
* Essentially, the issue was the blocks below it would explode using TNT, leading the MotherBoard into the void.
* Now, the blocks below it or around it will not explode.
* This only includes the blocks that are apart of the motherboard.

- Fixed MotherBoard from taking knockback upon TNT explosion to it.

- Added Obsidian Health Detector to Main shop.

- Added Flint And Steel to Main shop.

- Fixed flint and steel image from glitching in the UI.

- Added Auction House to the server!

- Added the following Auction House Commands:
* /ah shop - Opens the main AuctionHouse UI.
* /ah sell <price> - Sells an item in your hand for a certain price.
* /ah listings - Shows all active listings of the player.
* /ah categories - Opens category menu

- Added the following new information categories to the Main Info UI:
* Envoys (Includes rewards)
* Crates (Includes Rewards and how to get them)

- /spawn timer is now set to 3 seconds, instead of randomising the seconds.

- Added Enchantment Table floating text at spawn.

- Speeded up the Crates animation to x5.

- You can now get Miner keys from Miner Minion.

- Fixed minion upgrading levels from not working as intended.

- You can no longer PvP your allies.

- You can no longer PvP your island members.

- Spawner Levels are now Roman Number, which means instead of for example, Level 1, it'll now say Level I, and so on.

- TNT will no longer explode in areas that do not have an island claim.

- You can no longer raid your own base.
* This is simply so we can have a good feel of skyblock whilst still maintaining our factions part of the server.

**So how do we raid then?**
- You can be an insider, and give your coordinates to your friend so they can raid with you.

- Fixed being able to PvP your island members/allies.

- Fixed Crate from not closing sometimes after you opened it.

- You can now get MotherBoard rewards every 10 minutes.

- Fixed Per Player List from becoming broken.

- Added $ sign to one of the Crate opening's money rewards.

- Money rewards you obtain from crates will now turn into a Bank Note, instead of automatically adding it to your balance.

- Renamed Money rewards to add "Note" name to them.

- Add a comma inbetween thousands units in Crates opening and its money rewards.

- Added Anti-Door Glitch to the server!

- Those in creative mode can now bypass the Anti-Glitch system. This means you will not get teleported when you try to break blocks.

- Made Motherboard alive reward message more specific as to how long the core's been alive for.

**NOTE**
* Core, is a nickname for MotherBoard. Though it's actually a Motherboard, you can also call it Core if you wanted to.

- Improved Command glitching.

- Added /is ally chat.

- Added /rewards - Displays current rewards you've obtained, e.g Core rewards/raiding rewards, etc.

- Added /profile

- Added Minion Shop Category to /shop.

- Added /craft - Opens the Crafting Table Menu.

- Added /invsee

- Added /enderinvsee

- Added /pv

- Added /ci, which does the same thing as /clearinventory.

- Fixed Mage Minion from not spawning.

- You can now get $100 from killing players.

- All kill rewards will now go straight to /rewards.

- Fixed heart particles from always occurring, even when the Core regeneration activates.

- Fixed protected entity perk from becoming broken.

- Removed Linkable chests to Heal Minions.

- Heal Minion Radius is now set to 10 blocks.

- Added Player Vaults (/pv)

- Added back /invsee

- Added back /enderinvsee

- Fixed crash when using /invsee and /enderinvsee.

- Added AI to Essence Minion.

- Fixed Farmer bugs that occurred.

- Staff Commands + Permissions are finally complete!

- Separated Bans and Warns to make it their own UI, rather than using it all in one, as this caused bugs and confusions with it.

- Added the following commands:

- /warn
- /warnlist
- /warnlogs
- /warnhistory
- /unwarn

- Fixed crash when trying to join when banned.

- You will now get automatically banned if you leave the server whilst frozen.

- Fixed /is ally remove from not being able to remove you from the island.

- Fixed /is ally chat from not working as expected.

- Added new API Method: getMergedMembers().
* Essentially, this function merges the Island members and their ally members, merging it together, to make one method.
* This is useful for if you're in /is ally chat, and want to talk with your allies alongwith your island members.

- Added Pets to the server.
**HOW PETS WILL WORK?**
* Currently, there is no way of getting pets. But pets can be used to make your life literally x10 easier.
* Want to quick teleport to your island? Then no problem! Use the Island Pet item to teleport to your island.
* Want to add fire resistance to your effects? Cool! We've got that! Just use the Fire Resistance Pet.
* Want to jump around like a bunny? You can do that! Juse use the Rabbit Pet to get around!
* There are so much more you can do with pets. The pets limitation is endless, and we plan to add way more in the future.

- Added /lagclear - Clears the lag manually.

- Fixed not being able to place lava and water on your island.

- Fixed Core Rewards from not being obtainable by other islands.

- Allies no longer receive Core rewards as it isn't their core.

- We've finally replaced the island owner's name with the Island's name upon destroying the core.

- Fixed players being able to place minions whilst in a queue.

- Added Sell Boosters to the server.
**HOW IT WORKS?**
* So Sell Boosters, are boosters, where you can sell for a lot more money than if it was a default booster, which is 1.
* This helps so you can earn money quicker.

- Added new command: /pvp

- Fixed /pvp from becoming disabled temporarily.

- Fixed Sell Boosters boss bar message from not disappearing when removing your sell booster.

- Added **BRAND NEW** boss: Virus.
**HOW IT WORKS?**
* There is no way to obtain the boss, and it spawns every 3 hours in the PvP Arena.
* PvP for players are turned off whilst this boss fight event is happening.
* You can only teleport there once, so if you die, you can't go back there until everyone involved dies, or when the boss is defeated, then you can go to the arena.

- Fixed crash when attempting to open Virtual crate.

- Fixed virtual keys from not saving to the database.

- Added Custom Farming
**HOW IT WORKS?**
* Custom farming, is a new way of farming! Essentially, you can place crops where appropriate. Once you place it down, you'll notice some changes.
  
**PARTICLES**
* We have made it so particles appear when it's actually growing in real time, starting from 10 seconds.

**Floating Text, Custom made**
* We've made it so it now tells you how long before the crop fully grows.

**BRAND NEW INTERFACE**
* We now provide a way to check out your Crops status.
* You can click on the Crop to open a UI.
* In the UI, it only currently provides two things:
* 1. Removing a Crop/Sapling.
* 2. Close

- The good thing about this, is our ideas with this are literally endless.

- Fixed incorrect trees from growing.

- Added new Minion: LumberJack.
**HOW DOES IT WORK?**
* A lumberjack, is where it'll break all logs connected together, and add them to your linked chest.
* Because we're so unique, I've decided to add Custom Trees to the server.
**What is custom trees?**
* So in our case, custom trees are where all of the trees will automatically grow after the previous growth.
* Essentially, you place a sapling down, and it'll tell you in REAL TIME how long until it fully grows.

**Offline support?**
* So as tested, trees growing does and should provide offline support. Though, there are some things relating to this that do not have offline support.
* Currently, things like Minions WILL not work when you're offline. This is something we simply cannot fix, as this is due to chunks being unloaded.

- Added LumberJack to /shop

- I've made going to /shop so much easier now. Here's the changes we recently made for most parts of the shop:
* We've made confirmination of buying items a lot easier now, especially for those that wanted to buy minions.
* Before, you'd need to reopen the minion shop every time you buy something. Now, it'll stay on that page until you feel like you want to close out of the menu.
* We may support more than one item count for Minion shops in the future.
* We've also done this with things like Island shop, Enchantment shop, etc.
* I've also fixed wrong-closing form for certain parts of /shop.
* This basically means when you close the UI, it could appear in a random UI that you never visited.

- We've fixed up a shit ton of incorrect information with the /is UI. (May still be more to come).

- Using the full island arguments command will no longer send a input field, where you'll need to enter a player's IGN.
* As soon as you type the full argument, it'll recognize it easilly, and won't make you type it all over again. ;O

- Fixed /is accept and /is deny UI from actually being able to do it via the UI interface.

- We've made it so it messages you the error and the success message along with the Form UI opening.
* Essentially, before, when you typed /is accept <player>, sometimes the UI wouldn't display, and would then unable to find out what it said.
* Now, the messages will be sent in chat along with the Form UI for better  and easier understanding.

- Added the following new Island Commands:
* /is members
* /is banlist

- Added the following new Form UI's for /is:
* Island Allies -> Island Management category
* Island Fly -> Island Profile category.
* Island Find -> Island Profile Category.
* Island Members -> Island Management
* Island BanList -> Island Management

- We've added Allies information as well as your own island's information!

- Trees and crops will now instantly grow 60 seconds before a server restart occurs where possible.
* This is handy for those with minions, as they're always active regardless.
* The minions can mine the tree, which then re-activates the tree/crop timer again.

- Fixed new line issues in /is info.

- Fixed /is info <player> from always appearing as yourself's information, rather than the given player you entered's island information.

- Fixed crash when interacting with Dark oak and Acacia sapling, as those currently do not support growing trees on them.

- Unknown Sapling will now default it to Oak Saplings upon interaction.

- Fixed a bug, where you wouldn't be able to fully heal your core if it's close to full health.

- Fixed certain skyblock commands from breaking completely.

- Fixed /is create from not being able to create the island name, thus leading to an error.

- Fixed /is restart from not being able to restart with the new island name, thus leading to an error.

- Fixed /is rename from not being able to rename your island, thus leading to an error.

- Fixed /is description from not being able to add a description to your island, thus leading to an error.
- Added Fire wand.

- Fixed Fire wand from exploding island blocks.

- Added array_filter to our explosions. Coming soon, we may implement Async Explosions, which shouldn't lag as much whilst exploding.

- Use empty() instead of isset() in arguments with spaces, such as /is create, /is restart, /is rename, and /is description.

- Added a very cool system with island titles, where after it says which island you're on, it'll then say regarding doing /is info if you're interested as to who they are.

- Fixed Raiding alerts for allies.

- Fixed being able to raid your own allies/island's base.

- We've resorted TNT to ensure exploding doesn't lag the server.
* When we mean by not lag, this doesn't mean TNT its self won't lag the server if you have like 1,000 TNT.
* This means tnt won't lag the server if it's small amount, like 1 tnt, which before, would've caused a delay between its igniting and explosion phase.

- Fixed TNT from lagging the server.

- Fixed being able to bypass TNT explosions if ignited a lot of the tnt in the same area.

- Added new Function: canExplode()
* Whether or not the TNT can be exploded in that area/given area.
* Returns true if able to explode in that area, and returns false if tnt explosions are cancelled.

- SkyBlock::getPlayersAtIsland() parmeter can now be a string, instead of just a Player::class parmeter.

- Fixed bug where saplings would turn into oak saplings after server restarts.

- Block metas after 4 of saplings will now turn into their appropriate forms.

- Fixed MOTD from appearing with an incorrect Season.
* Before, the MOTD would display "S2" instead of S1. Now, this has properly been detected and fixed.

- Fixed double error messages when attempting to shoot yourself with a bow or a projectile.
* Before, both errors: "You cannot PvP your island members" and "You cannot hit yourself using a projectile" would occur.
* Now, we've made it so the Island members error doesn't occur if shooting yourself.

- Added Wands!
**How it works?**
* There are currently 6 types of wands.
* Each type has their own ability and effects.
* Here are the following effects we currently provide:
** Fire Wand - Shoots arrows that will burn your enemy.
** Explosion Wand - Allows explosive arrows upon hit.
**Speed Wand - Gives you and your allies speed.
**Growth Wand - Makes you and your allies bigger than other normal sized players.
**Blindness - Gives your enemy blindness.
**Poison - Gives your enemy poison.

- Fixed a bug, where wands wouldn't give enemies effects when they aren't in an island.

- Fixed a bug, where bad effective wands would go on yourself and your allies.

- Fixed crash when explosion death message attempts to appear.
* This was because we didn't have this type of death occurance in our configuration file.

- Fixed Viruses boss from spawning in more than one.
* This issue would've occurred when the chunks are unloaded, and it wouldn't recognize if there's more than one boss there.
* Before, it would've spawned in more than one virus boss because it wouldn't recognize if the chunks are unloaded.
* Now, it'll attempt to get rid of all the bosses until there's one left.
* We do this by fetching array_rand() in the boss class its self.

- Wands will no longer knock you back on good effective wands.

- Wands will no longer knock you back on bad wand effectives.
* The only time it'll do this, is if you're being damaged by them.

- Bad effective wands will no longer knock you back if you're their ally/apart of their island.

- Fixed /spawn timer from becoming broken, and unuseable.

- Fixed /pvp timer from becoming broken, and unuseable.

- Added BRAND NEW TUTORIAL MODE!
**How it works?**
* Once you're loaded into the server, a UI will appear, asking you if you'd like to know more about the gamemode. If you preceed to continue, it'll show you around the server.

- Moved /spawn command to the SkyFactions core.
* This is because /spawn is mainly for non-network gamemode server.
* This means /spawn is for servers like SkyFactions, rather than implementing /spawn to the Network core its self, which /spawn wouldn't be considered as appropriate for the network core.

- Fixed bug where it'd appear as the Tutorial Mode Request twice, once when joining, and the other when you load in the server.

- The Tutorial Mode Menu should no longer allow you to bypass being able to move.
* The reason why this occurred in the first place, is because onJoin() would occur, and you could select to go straight to tutorial mode, even if you're still in the queue.
* Another reason is because when you're loading into the server (As in loading data titled screen), you were able to go to tutorial that way, thus bypassing the system.
* Now, the UI will only appear 1-2 second after your data is fully loaded.

- You can now remove an ally even when the ally island leader is offline.

- Added /kit

- Finally added Donator kits to /kit!
**HOW IT WORKS?**
* Currently, you can only obtain donator kits. We may plan on adding more kits soon.
* Each kit comes with their own cosmetics!
* That's right! All donator kits will come with their own cosmetics you can use against your enemy!

- We've finished Player permissions! They're now all set up, and ready to go!

- We've finished Donator Permissions! They're now all set up, and ready to go!

- We've finished Staff permissions! They're now all set up, and ready to go!

- Added per item permission for staff mode, to reduce being able to use items that they shouldn't have access to.

- Fixed the following admin permissions:
* /givemoney
* /setmoney
* /takemoney
* /banknotes admin
* /gamemode
* /homeadmin

- Fixed the following Moderator permissions:
* /invsee
* /enderinvsee

- Players can now get banned if they're frozen and decide to leave the server.

- Fixed crash when pressing "No" in the Enchant shop confirmation UI.

- Fixed an issue where armor would always be put onto your armor slot when you right click/tap with the enchantment table.

- Added Grappling hook.
**How it works?**
* If you've been here since ZectorPE hub was released, then you've probably heard of "Grappling hooks".
* On ZectorPE, you could use Grappling hooks to get around places.
* On VirtualPE, you can use grappling hooks to get around, but to also get away from your enemies! It's essentially a cosmetic, useful for PvP.

- Crops will now appear as "Fully Grown" when it's grown fully, same applies to trees somewhat.

- Fixed /kick command from acting like /ban, alongside its display.

- /kick now works as intended.
* before, /kick wouldn't work, and would then keep asking for the reason of the kick, even if you've already entered a kick reason.
* Now, /kick will act appropriately, and kick the user if a reason is entered.

- Fixed issue where staff weren't able to bypass the queue system.

- Only staff can now join the server when it's full. We may add this for donators in the future. (To be confirmd).

- Fixed Cheetah pet from not being functional.

- Fixed Fire Pet from not being functional.

- You can now only obtain one kit per 24 hours.
* This is something we really wanted to do for quite some time now.
* This also prevents having too much cosmetics in your inventory.
* Essentially, comparing it to ZectorPE, it's a lot different.
* ZectorPE - You could claim more than one kit per cooldown.
* VirtualPE - You can only claim one kit per 24 hours, thus discludes multiple kits at once.
* ZectorPE - Staff could claim all kits at once, without a cooldown.
* VirtualPE - Staff will be included in a one kit only system.
* This means staff will have to be involved in the same way as players and donators do - Using a one kit per 24 hours cooldown.
* I think we're one of the only servers that provide this, hence why we're the #1 best unique skyblock + factions based servering network.

- Improved on Pet effects, make them a bit longer.

- Added cooldown for Grappling hooks to 20 seconds.

- Reduced forever effects amplifier for Donators to Haste 1, and Night Vision 1.

- Changed the ranks display in-game to make it look more professional.

- Fixed chat formatting from messing its chat color with chat formatting.

- Added all permissions to ranks.

- Renamed Partner rank to Influencer rank in-game and on discord.

- Fixed Explosion wand from being too overpowered!

- Added the following new kits:
* Starter Kit
* Influencer Kit.
* Fixed kit cooldown from becoming broken.

- Moved Nether star to above and below Reward item.
* This is so it's easier to understand where the reward item really is.

- Fixed Spawners from not being functional.

- Fixed crash when attempting to use /shop, and clicking "No" confirmination for Island shop.

- Tutorial Menu will now only appear when a user has joined for the first time.

- Explosion Wand is wayy less OP than before.

- Fixed bug where going into the void will put you in Visiting mode, even though you never visited the island using /is visit.

- Fixed /verify on our discord server.

- Fixed Virus Boss from reaching too far.

- Fixed Virus boss from its reach becoming too low.

- Added /boss, which states how long before a boss spawns!

- Fixed not being able to obtain Unbreaking Enchantment from Enchantment shop category in /shop.

- Having more than one XP Bottles will now automatically add up to your xp balance, and remove all of the XP Bottles, instead of doing it one by one, thus making it longer and hard for you.
h
- Fixed crash when attempting to add your XP due to Mending.

- We've changed how the queue system hides players. It'll now hide them a lot efficiently now.

- Added Invisibility particles to the queue system.
**HOW IT WORKS?**
* When you're put in the queue, the invisibility effect will be added to you.
* The duration does depend on the queue time.
* For example, if the queue time is at 5 seconds, you'll have your invisibility effect for 5 seconds.
* This fixes a lot of bugs relating to players that are able to get in a higher queue position, which if they both spawned at the same time, one wouldn't be able to see the other, or even both of them!
