# Playit.gg Minecraft mod

> [!WARNING]  
> While this mod works, it is recommended to use the playit program instead if possible as this offers more features and better routing (which can reduce overall latency)

**Disclaimer**: This is an unofficial mod and is not affiliated with Playit.gg.

[Modrinth Page](https://modrinth.com/mod/playit-gg)
[Curseforge Page](https://legacy.curseforge.com/minecraft/mc-mods/playit-gg)

This mod will make your server, or singleplayer world public using the [Playit.gg](https://playit.gg) network, without having to port forward.

## Installation

1. Download the latest release from [here](https://github.com/maxomatic458/playit-forge/releases/latest)
   (fabric version requires [Fabric API](https://www.curseforge.com/minecraft/mc-mods/fabric-api))
2. Put the downloaded jar file into your mods folder

3. Follow the instructions in your chat/server console
   (If you are in a singleplayer world run ``/playit open-lan``)

5. You will get a static IP and Port, that anyone can use to connect to your server

## Commands
- ``/playit``
  - ``open-lan``, make your singleplayer world public
  - ``agent``
    - ``status`` get the current status of your playit connection
    - ``restart`` restart the playit connection-manager
    - ``reset`` unbind the mod from your playit.gg account
    - ``shutdown`` stop the connection to playit (existing connections will stay open, until closed)
    - ``set-secret`` manually set the secret of the playit mod

  - ``prop``
    - ``set <option> <value>`` set a config option
    - ``get <option> <value>`` get a config option
  - ``tunnel get-address`` get the address of the mods playit tunnel (the address your players use to connect with)
  - ``account guest-login-link`` generate a link to connect the mod to a playit.gg guest account

**config options**

``mc-timeout-secs`` timeout in seconds for the tunnel channel (default 30s)

``autostart`` whether playit should automatically start with your server or singleplayer world (default server: true, client: false)

### Other Links
* [Playit bukkit plugin](https://www.spigotmc.org/resources/playit-gg.105566/) (this mod is basically a forge translation of this plugin)
* [Playit program](https://github.com/playit-cloud/playit-agent)
