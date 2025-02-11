# Welcome To Hydra Ui Library!

# Booting The Lib
```lua
local UILib = loadstring(game:HttpGet('https://raw.githubusercontent.com/StepBroFurious/Script/main/HydraHubUi.lua'))()
```

# Window 
```
local Window = UILib.new("Grand Piece Online", game.Players.LocalPlayer.UserId, "Buyer")
```

# Category
```lua
local Category1 = Window:Category("Main", "http://www.roblox.com/asset/?id=8395621517")
```

# Sub Button
```lua
local SubButton1 = Category1:Button("Combat", "http://www.roblox.com/asset/?id=8395747586")
```

# Section
```lua
local Section1 = SubButton1:Section("Section", "Left")
```

# Button
```lua
Section1:Button({
    Title = "Kill All",
    ButtonName = "KILL!!",
    Description = "kills everyone",
    }, function(value)
    print(value)
end)
```
# Toggle
```lua
Section1:Toggle({
    Title = "Auto Farm Coins",
    Description = "Optional Description here",
    Default = false
    }, function(value)
    print(value)
end)
```

# Slider
```lua
Section1:Slider({
    Title = "Walkspeed",
    Description = "",
    Default = 16,
    Min = 0,
    Max = 120
    }, function(value)
    print(value)
end)
```

# Color Picker
```lua
Section1:ColorPicker({
    Title = "Colorpicker",
    Description = "",
    Default = Color3.new(255,0,0),
    }, function(value)
    print(value)
end)
```

# Text Box
```lua
Section1:Textbox({
    Title = "Damage Multiplier",
    Description = "",
    Default = "",
    }, function(value)
    print(value)
end)
```

# Keybind
```lua
Section1:Keybind({
    Title = "Kill All",
    Description = "",
    Default = Enum.KeyCode.Q,
    }, function(value)
    print(value)
end)
```
