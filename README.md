# Misc

```diff
local uilibrary = loadstring(game:HttpGet("https://raw.githubusercontent.com/LiterallyATrueClown/SeaHubFake/main/SeaHubUILIBFake.lua", true))()
```

# Create Window
```lua
local windowz = uilibrary:CreateWindow("Sea Hub", true)
```
# Create Tab
```lua
local Page1 = windowz:CreatePage("Main")
local Section1 = Page1:CreateSection("Misc Features")
```
# Button
```lua
Section1:CreateButton("Redeem all EXP Codes", function ()
	print("Button Cliked!")
end)
```
# Toggle
```lua
Section1:CreateToggle("Auto Rejoin", {Toggled = false , Description = "Auto Rejoin if got kicked (this doesn't work with Private Server)"}, function(Value)
	print(Value)
end)
```
# Dropdown
```lua
Section1:CreateDropdown("Dropdown ", {
	List = {"Value1", "Value2", "Value3", "Value4"},
	Default = "None"}, function(value)
	print(value)
end)
```
# Label
```lua
local A = Page:Label('Label') --name
local B = Page:LabelLog('Label') --name
```
# Set Label 
```lua
A:Refresh("A") -- name
B:Refresh("B") -- name
B:Color(Color3.fromRGB(255, 255, 255))  -- Color
```
# Slider
```lua
Section1:CreateSlider("Slider Example", {Min = 16, Max = 500, DefaultValue = 30}, function(Value)
	print(Value)
end)
```
# TextBox
```lua
Section1:CreateTextbox("TextBox", false, function (vv)
	print(vv)
end)
```
# CreateColorPicker
```lua
Section1:CreateColorPicker("Color Picker", Color3.fromRGB(255, 255, 255), function (uwu)
	print(uwu)
end)
```
# CreateKeybind
```lua
Section2:CreateKeybind("Keybind", "T", function(key)
	print("Pressed "..tostring(key))
end)
```
