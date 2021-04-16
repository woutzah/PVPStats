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

- v1.7.42 - sync with master v1.9.4
  - **FEAT**: add configurability for numbered entries, support player meta tags (NPC) to exclude from statistics
  - **FEAT**: add ability to run multiple commands on a streak
  - **FEAT**: introduce K/D interpreter - it supports powers `x² => (x^2)` - thanks to garbagemule for the inspiration
  - **FEAT**: Add new config setting 'shortHandCommands' to disable exclamation point shorthand functionality
  - **FEAT**: Introduce pvpstats.show to restrict players watching other players' stats
  - **FIX**: shift the logic around to make meta restrictions work
  - **FIX**: run streak commands synchronously!
  - **FIX**: allow to count pet kills, fix newbie check for deaths not from PVP
  - **FIX**: hide ELO information in outputs if ELO is not activated
  - **FIX**: use plugin prefix in more places, this should reduce confusion and clarify who is talking
  - **FIX**: properly treat the "simple calculation" config node as boolean
  - **FIX**: teach K/D interpreter to display a number that makes some sense rather than 0, when dividing by 0
  - **FIX**: take minimum and default ELO into account when creating player statistics; fix test logic
  - **FIX**: Replace hardcoded messages with language messages
- [read more](doc/changelog.md)

***

## Phoning home

By default, the server contacts www.bstats.org to notify that you are using my plugin.

Please refer to their website to learn about what they collect and how they handle the data.

If you want to disable the tracker, set "bStats.enabled" to false in the __config.yml__ !

***

## Support

I am developing this plugin in my free time, so if you have an issue, please create an issue describing the problem in detail. I will do my best to reply as soon as possible, but that can take a few days sometimes.

For some problems, it might be easier to join the [Discord](https://discord.gg/DSNfjYA) and open a ticket there. It allows for quicker transfer of log files, debug files and so on. Moreover, simple questions can be answered more quickly there rather than opening an issue for them.

Joining the Discord Server gets you early access to latest builds, and maybe it is your preferred method to interact with me? Be my guest!

***

## Credits

- pandapipino for the idea


***

## Todos

- Move language nodes into proper block logic

***