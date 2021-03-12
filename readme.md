# PVP Stats

**Keep track of your users' PVP actions - MySQL or SQLite recommended**

This plugin will keep records of how many kills, deaths, kills in a row a player has, and possibly keep an ELO score.

***

## Features

- Records kills, deaths, max streaks, current streak, kill/death ratio

### Options

- MySQL support (highly recommended)
- SQLite support
- ELO score calculation
- PVP Arena integration

***

## Dependencies

- Spigot 1.8 through Spigot 1.12

***

## Downloads

- [spigotmc.org](https://www.spigotmc.org/resources/pvp-stats.59124/)
- [Discord - #pvpstats-builds](https://discord.gg/BNkk46vRKa)


***

## How to install

- Stop your server
- Place jar in plugins folder
- Run a first time to create config
- Configure database settings
- Reboot again, done!

***

## Documentation

- [API](doc/api.md)
- [Commands](doc/commands.md)
- [Permissions](doc/permissions.md)
- [Configuration](doc/configuration.md)
- [LeaderBoards](doc/leaderboards.md)

***

## Changelog

- v1.7.41 - sync with master v1.8.10
    - **FIX**: fix server crash when looking up player info on async compatible systems
    - **FIX**: IDEA calls this "performance"
    - **FIX**: fix debug "all"
    - **FIX**: hotfix: fix crashes for mysql users
    - **FIX**: update version check to work with alpha testing builds
    - **FIX**: remove api version in plugin.yml, this was introduced in 1.13
    - **FEAT**: change default behavior for precise stats to not run. there is an override config setting that will be announced instead of a warning that no-one listens to
    - add debug logs for async or sync
    - add discord dev build link
- [read more](doc/changelog.md)

***

## Phoning home

By default, the server contacts www.bstats.org to notify that you are using my plugin.

Please refer to their website to learn about what they collect and how they handle the data.

If you want to disable the tracker, set "bStats.enabled" to false in the __config.yml__ !

***

## Credits

- pandapipino for the idea


***

## Todos

- Move language nodes into proper block logic

***