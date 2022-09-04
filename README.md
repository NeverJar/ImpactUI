# ImpactUI

ImpactUI is an beautiful UI Library for Roblox Script using Lua!
Its have a Dark and Blurple Design and its easy to learn!

<img src="https://i.imgur.com/U120piK.png" width="500" />

## Usage

### Basics

To import the Library you need to enter these
```lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/NeverJar/ImpactUI/main/ImpactUI.lua"))()
```

Then u need to create a Window using this:
```lua
local Window = Library:Create("Hub Name", "Game Name")
```

### Creating a Tab

```lua
local Tab = Window:Tab("Tab Name", true)

--[[
  NAME: STRING
  VISIBILITY: BOOLEAN
]]
```

### Creating Labels

```lua
Tab:Label("TEXT")

--[[
  TEXT: STRING
]]
```

### Creating Buttons

```lua
Tab:Button("Button Name", function()
    -- Code here
end)

--[[
  NAME: STRING
]]
```

### Creating Textbox

The variable in the function will be the text.

```lua
Tab:Textbox("Name", "Placeholder", function(txt)
    -- Code here
end)

--[[
  NAME: STRING
  PLACEHOLDER: STRING
]]
```

### Creating Keybinds

```lua
Tab:Keybind("Keybind Name", Enum.KeyCode.G, function()
    -- Code here
end)
```

### Creating Dropdowns

You can do with current an if statement!

```lua
Tab:Dropdown("Dropdow Name", {"Option 1", "Option 2", "Option 3"}, function(current)
    -- Code here
end)

--[[
  NAME: STRING
  OPTIONS: STRING LIST
]]
```

### Creating Toggles

```lua
Tab:Toggle("Toggle Name", function(bool)
    -- Code here
end)

--[[
  NAME: STRING
]]
```

### Creating Sliders

```lua
Tab:Slider("Slider Name", 16, 500, function(value)
    -- Code here
end)

--[[
  NAME: STRING
  MIN-VALUE: INT
  MAX-VALUE: INT
]]
```

### Show/Hide Window

```lua
Library:Toggle()
```
