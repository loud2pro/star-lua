## NOTICE: This hasn't been released to public versions of Star yet, as it is still in very early testing (and lacks a lot of features.)

# star-lua
Documentation for Star's Lua Scripting API.
**This will show you every current function that can be used in the scripting API, with examples**
## Initializing a Game instance
Game.new returns a instance of the Game.
```lua
<LuaGame> Game.new(<void>)
```
## Initializing a Player instance
Player.new returns a instance of the Local Player.
```lua
<LuaLocalPlayer> Player.new(<void>)
```

# LuaGame
## Sending a message to client chat
LuaGame::send_client_message will display a message to you, clientsidedly
```c++
<void> LuaGame::send_client_message(<string> message)
```
### Example:
```lua
local game = Game.new()

game:send_client_message("Hello from the Star scripting API")
```
## Sending a message to global chat
LuaGame::send_chat will display a message to you, clientsidedly
```c++
<void> LuaGame::send_chat(<string> message)
```
### Example:
```lua
local game = Game.new()

game:send_chat("Hello from the Star scripting API")
```

# LuaLocalPlayer
## Swinging your arm
LuaLocalPlayer::swing will swing your arm
```c++
<void> LuaLocalPlayer::swing(<void>)
```
### Example:
```lua
local lp = Player.new()

lp:swing()
```
