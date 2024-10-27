## Create Window
```lua
local lib = loadstring(game:HttpGet("https://raw.githubusercontent.com/ydntsdfprnartytva/ViseUI/refs/heads/main/source"))()
```
## Create Tab
```lua
local tab1 = lib:NewTab{name = "Catching"}
```
## Create Section
```lua
local sec1 = tab1:NewSection({name = "Mags"})
```
## Create Toggle
```lua
tab1:Toggle({
	name = "Regular Mags",
	default = false,
	flag = "Toggle",
	callback = function(v)

	end,
})
```
## Create Slider
```lua
tab1:Slider({
	name = "Regular Mags Strength",
	min = 2,
	max = 25,
	default = 10,
	callback = function(v)

	end,
})
```
## Create ColorPicker
```lua
tab1:Colorpicker({
    name = "Choose Color",
    default = Color3.fromRGB(255, 255, 255),
    callback = function(selectedColor)
        print("Selected Color: " .. tostring(selectedColor))
    end
})
```
## Create Dropdown
```lua
tab1:Dropdown({
    name = "Select Option",
    option1 = "Option 1",
    option2 = "Option 2",
    option3 = "Option 3",
    default = "Option 1",
    callback = function(selectedValue)
        print("Selected Value: " .. selectedValue)
    end,
})
```
