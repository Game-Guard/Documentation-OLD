# Adding No Clip Exclusions
This function will allow you to add a players no clip exclusion parts.

## Parameters:

| Parameter     | Description                                                | Type   |
|---------------|------------------------------------------------------------|--------|
| plr           | The player of which the no clip part will be excluded for. | Player |
| excludeObject | The part that will be excluded in no clip for the player.  | Part   |

## Example Usage:

```lua
local gameGuard = require(script.Parent.gameGuard)
local Players = game:GetService("Players")

Players.PlayerAdded:Connect(function(plr)
    gameGuard:init(plr)
    gameGuard:ncAddExclusion(player, Workspace:WaitForChild("Exclude")) -- Will exclude part in workspace called "Exclude".
end)
```