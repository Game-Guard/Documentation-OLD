# Initialize

# Parameters:

| Parameter | Description                                              | Type   |
|-----------|----------------------------------------------------------|--------|
| plr       | The player object in which to initialize Game Guard for. | Player |

# Example Usage:

```lua
local gameGuard = require(script.Parent.GameGuard)

game.Players.PlayerAdded:Connect(function(plr)
    gameGuard:init(plr)
end)
```