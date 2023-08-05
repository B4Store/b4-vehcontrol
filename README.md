# New Design

* Preview ( `https://cdn.discordapp.com/attachments/1063743188734574632/1136439381050261575/preview_1.png` )

# Discord ` https://discord.gg/b4s `
# Discord ` https://discord.gg/NvbDy6j4Qd `

# Add This in Your Radialmenu
```lua
{
        id = "general:vehicle",
        displayName = "تحكم السيارة",
        icon = "#car",
        functionName = "vehcontrol:openExternal",
        enableMenu = function()
            local src = source
            local Player = QBCore.Functions.GetPlayerData(src)
            local inlaststand = Player.metadata["inlaststand"]
            local isdead = Player.metadata["isdead"]

            return not isdead and not inlaststand and IsPedInAnyVehicle(PlayerPedId(), true)
        end
    },
```

# And This is event For open if you use any radial menu
```lua
`vehcontrol:openExternal`
```

# Discord ` https://discord.gg/b4s `
# Discord ` https://discord.gg/NvbDy6j4Qd `