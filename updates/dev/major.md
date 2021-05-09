## VirtualPE Development updates:

## This changelog introduces a new and complete Core revamp, along with: Major API changes (API BC), and many changes with the concurrent server.

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
How far tho?
Level 1 - 15 Blocks for 30 Essences
Level 2 - 18 Blocks for 60 Essences
Level 3 - 21 Blocks for 90 Essences

- Well, they simply break. They do not disappear, no you can pick their Pieces up! Essences and iron blocks!

You can obtain 2 Essences and 5 Iron blocks from them dropping!


## How do you obtain them?

- You can craft it using iron blocks and essences, which will come hopefully in the next update!
