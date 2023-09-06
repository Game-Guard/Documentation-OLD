# Getting Version

## Parameters:

| Parameter | Description | Type |
| --------- | ----------- | ---- |
| None      | None.       | nil  |

## Example Usage:

```lua
local gameGuard = require(script.Parent.gameGuard)
local Players = game:GetService("Players")

Players.PlayerAdded:Connect(function()
    print(gameGuard:getVersion()) -- Will print table:
        -- {
        --     ["version"] = version, -- The version of Game Guard.
        --     ["tag"] = tag, -- The current tag of Game Guard.
        -- }
end)
```
