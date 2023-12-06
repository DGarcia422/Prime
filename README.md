# Prime server scripts

### Teleport by coordinates
```
local destinationCoords = vector3(x, y, z)
local playerId = GetPlayerFromServerId(playerId)
SetEntityCoordsNoOffset(GetPlayerPed(-1), destinationCoords.x, destinationCoords.y, destinationCoords.z, true, true, true)
```

### Rob any player (replace "playerId" with the targets ID)
```
TriggerServerEvent("inventory:server:OpenInventory", "otherplayer", "playerId")
```

### Coffee that speeds up task bars
```
TriggerServerEvent('inventory:server:CraftItems', "highnoon",{stones=0},10,1,5)
```

### All materials from washing stone
```
TriggerServerEvent('inventory:server:CraftItems', "uncut_ruby",{stones=0},19,1,5)
TriggerServerEvent('inventory:server:CraftItems', "uncut_emerald",{stones=0},28,2,5)
TriggerServerEvent('inventory:server:CraftItems', "uncut_diamond",{stones=0},23,3,5)
TriggerServerEvent('inventory:server:CraftItems', "uncut_sapphire",{stones=0},24,4,5)
TriggerServerEvent('inventory:server:CraftItems', "goldore",{stones=0},45,5,5)
```

### All gems(cut) from mining
```
TriggerServerEvent('inventory:server:CraftItems', "ruby",{stones=0},15,6,5)
TriggerServerEvent('inventory:server:CraftItems', "emerald",{stones=0},28,7,5)
TriggerServerEvent('inventory:server:CraftItems', "diamond",{stones=0},13,8,5)
TriggerServerEvent('inventory:server:CraftItems', "sapphire",{stones=0},19,9,5)
```

### Fully upgrade vehicles (Untested) Might ban
```
RegisterNetEvent("Pug:client:AdminFullyUpgradeCar", "2")
```
