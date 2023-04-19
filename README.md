# NOTICE: This hasn't been released to public versions of Star yet, as it is still in very early testing (and lacks a lot of features.)

# star-lua
Documentation for Star's Lua Scripting API.
**This will show you every current function that can be used in the scripting API, with examples**
## Initializing a Game instance
Game.new returns a instance of the Game.
```lua
<LuaGame> Game.new(<void>)
```
## Sending a message to chat
LuaGame::send_message will display a message to chat
```c++
<void> LuaGame::send_message(<string> message)
```
### Example:
```lua
local game = Game.new()

game:send_message("Hello from the Star scripting API")
```
