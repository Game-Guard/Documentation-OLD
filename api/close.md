# Closing Game Guard
This will close all loops and checks that Game Guard calls. **You should call this when a player leaves, suggested in the example below**.

## Parameters:

| Parameter | Description                                         | Type   |
| --------- | --------------------------------------------------- | ------ |
| plr       | The player object in which to close Game Guard for. | Player |

## Example Usage:

```lua
local gameGuard = require(script.Parent.GameGuard)
local Players = game:GetService("Players")

Players.PlayerRemoving:Connect(function(plr)
    gameGuard:close(plr)
end)
```