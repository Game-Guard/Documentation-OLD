# Check Speed

## Parameters:

## Example Usage:

```lua
local gameGuard = require(script.Parent.gameGuard)
local Players = game:GetService("Players")

Players.PlayerAdded:Connect(function(plr)
    local WalkSpeed = 16
    gameGuard:checkSpeed(plr, WalkSpeed, function(result)
        print(result) -- Will print true if the player is over the speed, vice-versa for if they are under the speed.
    end)
end)
```
