# Call Of Duty 2 - server documentation
Full credit goes to http://anarchyrules.co.uk/cod2/server%20commands.html 

## Map Name
All maps are available in each gamemodes:
- DM: death match
- TDM: team death match
- SD: search & destroy
- CTF: capture the flag
- HQ: headquarter

Map name list:
- mp_breakout
- mp_brecourt
- mp_burgundy
- mp_carentan
- mp_dawnville
- mp_decoy
- mp_downtown
- mp_farmhouse
- mp_leningrad
- mp_matmata
- mp_railyard
- mp_toujane
- mp_trainstation

## Console Commands

Here are the available commands you can use in the server terminal.

You can use commands in-game from the console: add the `/rcon` prefix and allow in-game console in server settings. Carreful not leaking your password when rcon login !

### rcon
* **/rcon login [rconpassword]**:
Login to remote rcon. 

### Common
* **status**:
Displays info of all the players on the server.
* **serverinfo**:
Shows the current server's settings.
* **systeminfo**:
Shows the current system information.
* **tell [id]**:
Sends private message to specified client id
* **say**:
Broadcast a message to all players
* **exec [FILENAME]**:
Executes a Server Config File (located in your server's main directory) 
* **writeconfig [FILENAME]**:
Saves a Server Config File 

### Gameplay
* **matchtimeout**:
Calls a match timeout (see server cvars for timeout settings)
* **matchtimein**:
Cancels timeout
* **setkillcam**:
Set the killcam cvar (now that it is read only during play)
* **setfriendlyfire**:
Set the friendly fire cvar (now that it is read only during play)
* **setdrawfriend**:
Set the draw friend cvar (now that it is read only during play)


### Map commands
* **map mapname**:
Loads the map specified by mapname.
* **map_rotate**:
Loads next map in rotation set in sv_maprotation.
* **map_restart**:
Restarts the map.

### Kick/ban Commands
* **kick [name]**:
Kicks a player by name from the server. (Must include Color Codes) 
* **rcon onlykick [name]**: 
Kicks a player by name from the server. (Does not need Color Codes) 
* **clientkick [id]**:
Kicks a player by client id from the server.
* **kick all**:
Kicks all players from server
* **banUser [name]**:
Bans a user by their ingame name. Writes their GUID to ban.txt
* **banClient [id]**:
Bans a user by their client number. Writes their GUID to ban.txt
* **tempBanUser [name]**:
Kicks and temporarily bans player by name from server.
* **tempBanClient [id]**:
Kicks and temporarily bans player by client id from server
* **unban [name]**:
Unban every player banned with [name]. If you want to unban a single player whose name appears more than once, you should edit "ban.txt" manually.



