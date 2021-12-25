# Nebula
A system used for administrating and operating ROBLOX games.

## Why Nebula?

Unlike most similar systems, Nebula allows for command and rank modification in-game, with libraries allowing for client-sided execution. Nebula also has been built with only two original Instances.

## How does it work?

First of all, the client executes a command. The server does parses the command and checks player permission level. If successful, the server executes the command, with code possibly firing the client again.

All atring execution is done by a built in Loadstring function from Yueliang.

## Framework

### Global Permissions

Usually, a rank has a number for the permission level. There are some exceptions.

Everyone, the default level.
Superuser, the highest possible level.

### Security

Commands do not have permission to the following:

- Framework key for DataStores.
- Ranks
- Modifying commands
- Framework client-server signals.
