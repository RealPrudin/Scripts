local library = loadstring(game:HttpGet(('https://raw.githubusercontent.com/AikaV3rm/UiLib/master/Lib.lua')))()

local CHSim = library:CreateWindow("Coins Hero Simulator")
local Autofarm = CHSim:CreateFolder("Autofarm")
local Credits = CHSim:CreateFolder("Credits")

local autoSelltoggle = false
Autofarm:Toggle("Auto sell",function(bool)
autoSelltoggle = bool
end)

spawn(function()
while wait()do
if autoSelltoggle then
    game.workspace.Lobby.Detect.Sell.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
end
end
end)

local coinstoggle = false
Autofarm:Toggle("Tp to coins",function(bool2)
coinstoggle = bool2
end)

spawn(function()
while wait() do
if coinstoggle then
local children = workspace.Coins:FindFirstChild("1"):GetChildren()
for _, child in pairs(children) do
for _, child in pairs(child:GetChildren()) do
end
if child:IsA("BasePart") then
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = child.CFrame
end
end
end
end
end)

Credits:Label("Made by Prudin#6667",Color3.fromRGB(38,38,38),Color3.fromRGB(0,216,111))
