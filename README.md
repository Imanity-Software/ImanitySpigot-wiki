# ImanitySpigot

![](https://i.imgur.com/F5BNaJV.jpg)

The 1.8.8 paper spigot fork, Focus on pvp, performance and api improvement

* [McMarket](https://www.mc-market.org/resources/10770/)
* [Discord](https://discord.gg/GBZKR3n)

![](https://i.imgur.com/lQgR1yZ.png)
- 1.8.8 PaperSpigot based, but with 1.7-1.15.2 client compatibility. (ViaVersion & ViaRewind Built-In)
- Automatic updater, the server will automatically download the server jar and other libraries if there is a new version available. It means you don't have to redownload everything whenever we push an update to the MC-Market.
- Configurable Cave Generation (Badlion 6.0 Cave), you can configure how will your [all] ores in the world to be generated.
- Knockback Modules, we provide various Knockback modules which give diverse algorithms according to different modes, that will maximize the server owner's experience toward their knockback configuration. There is also an developer API such that you could potentially create your own knockback algorithm and apply it in your iSpigot. By default, iSpigot provides 3 algorithms.
    Regular (Recommended, simple to configure)
    MinemenClub (Attempts to replicate MinemenClub knockback)
    Advanced (Based on Regular module, provides more configurable options such as rod knockback and bow knockback)
- Knockback Profiles, all of the knockbacks are profile-specific, which means that you can link a player to an unique knockback profile for them to play on (Extremely good in Practice servers)
- Asynchronous [Parallel] World Management, all of the world related things are being moved off from main thread, also break down into various workers to improve the server performance. (For example, you won't experience as much lag as you have 3 worlds compared to 10 worlds)
- Asynchronous Hit Detection, all of the attack packets are being sent without doing an extra load in main thread, this can make the hit detection smoother to improve the PVP Experience.
- Asynchronous [Parallel] Entity Tracker, all of the entity tracker updates are being accomplished asynchronously and will be breaking down into multiple workers to reduce the main thread's load.
- Asynchronous player NBT data saving, according to original spigot, all of the player NBT data's I/O operation are being accomplished in the main thread, iSpigot moved that action to another thread to make sure the server's thread has less work to do.
- MovementHandler, PacketHandler & AIHandler! You can create your own implementation of those handlers to control your server to a next level. (Perfect for Anti-Cheat plugin developments)
- 7 Built-in TNT Optimization, 4 of them are configurable. We cache the all possible velocities that a TNT is going to land to prevent numerous useless and massive math calculations.
- Configurable Client-Side FPS Boost (Invisible Primed-TNT, Falling Sands / Gravels, etc.)
- Configurable Taliban Pearls (Like Ve*t, etc.)
- Implementation of Panda-Wire Redstone Algorithm to improve the server's Redstone mechanics experience.
- Asynchronous Entity Pathfinder, all of the entity AI related methods are done off-main thread. It reduces the main server's load to another level depends on how much entities do you have in the server.
- World biome generation options, you can configure what biomes you want in a world without any external plugins. 
- Vanish Patch, all of the players are also prevented from seeing a vanished player's projectiles, items dropped, experience orbs, etc. (Extremely helpful for a practice server which has multiple matches in one arena)
- Developer Friendly, we integrated an extensive API for server developers to use.
- General network optimizations (For instance, TCP No Delay Enabled, Cached NetworkManager connection, etc.)
- Other configurations are waiting for you to discover..

bStats:

![](https://bstats.org/signatures/bukkit/iSpigot.svg)
