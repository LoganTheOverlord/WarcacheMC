**Bungee Security - a big topic**

How do I secure bungee server, so login can not be bypassed?
Only free solution is using AuthMe + AuthMeBungee
You must set auth/login server, where player logs in, and then, is sent to main lobby server.

How do I protect server from unathorised bungee connect?
For majority of existence of bungee, there is one known exploit - adding bungee server to your own instance of bungeecord, by which, you can connect to that server directly.
In order to avoid this, we use BungeeGuard. You put it on the bungee server (proxy), and on all it's sub-servers - minigames, survival, etc. You sync a key you create, or define, and you are done. Noone can connect to any server without knowing what key bungeeguard has.
On proxy, it has no effect. On servers, it won't let you connect without passing the key in.

How do I connect LuckPerms to bungee?
There are two downloads of LuckPerms - bukkit/spigot - and bungee.
* First, create a database on your hosting
* Go into luckperms config, and enter credentials for your database
* On each server, enter same info, and change server name/identifier respectively.
* Type /lp sync to sync the permissions.
* To modify bungee permissions, use /lpb, for spigot, use /lp.
* Those permissions are shared, thus, you assign both into one database, and every user has both bungee and spigot permissions, as granted in group.
