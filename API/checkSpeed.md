# Check Speed

## Parameters:

| Parameter | Description                                                     | Type     |
|-----------|-----------------------------------------------------------------|----------|
| plr       | The player object of which to check the speed value of.         | Player   |
| WalkSpeed | The amount of walk speed the detection will be run at.          | Int      |
| Result    | The function to call on the result of the check speed function. | function |

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
