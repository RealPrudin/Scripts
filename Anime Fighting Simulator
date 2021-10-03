local library = loadstring(game:HttpGet(('https://raw.githubusercontent.com/AikaV3rm/UiLib/master/Lib.lua')))()

local AFS = library:CreateWindow("Anime Fighting Simulator")

local Autofarm = AFS:CreateFolder("Autofarm")
local Other = AFS:CreateFolder("Other")
local Credits = AFS:CreateFolder("Credits")

local strengthtoggle = false
Autofarm:Toggle("Strength",function(bool1)
strengthtoggle = bool1
end)

spawn(function()
while wait(0.1)do
if strengthtoggle then
    game:GetService("ReplicatedStorage").RSPackage.Events.StatFunction:InvokeServer("Stat", "Strength")
end
end
end)

local durabilitytoggle = false
Autofarm:Toggle("Durability",function(bool2)
durabilitytoggle = bool2
end)

spawn(function()
while wait(0.1)do
if durabilitytoggle then
    game:GetService("ReplicatedStorage").RSPackage.Events.StatFunction:InvokeServer("Stat", "Durability")
end
end
end)

local chakratoggle = false
Autofarm:Toggle("Chakra",function(bool3)
chakratoggle = bool3
end)

spawn(function()
while wait(0.1)do
if chakratoggle then
    game:GetService("ReplicatedStorage").RSPackage.Events.StatFunction:InvokeServer("Stat", "Chakra")
end
end
end)

local swordtoggle = false
Autofarm:Toggle("Sword",function(bool4)
swordtoggle = bool4
end)

spawn(function()
while wait(0.1)do
if swordtoggle then
    game:GetService("ReplicatedStorage").RSPackage.Events.StatFunction:InvokeServer("Stat", "Sword")
end
end
end)

Autofarm:Label("For sword you will need to have it in your hand and also you can only do one at a time",Color3.fromRGB(38,38,38),Color3.fromRGB(0,216,111))

Credits:Label("Made by Prudin#6667",Color3.fromRGB(38,38,38),Color3.fromRGB(0,216,111))

Other:DestroyGUI()

Other:GuiSettings()
