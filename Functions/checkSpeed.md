# Check Speed

## Parameters:

## Example Usage:

```lua
local gameGuard = require(script.Parent.gameGuard)
local Players = game:GetService("Players")

Players.PlayerAdded:Connect(function(plr)
    gameGuard:checkSpeed(plr)
end)
```
