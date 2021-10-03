local library = loadstring(game:HttpGet(('https://raw.githubusercontent.com/AikaV3rm/UiLib/master/Lib.lua')))()

local Modded = library:CreateWindow("A Modded Destroyer")
local Money = Modded:CreateFolder("Money")
local Wrk = game.Workspace:GetChildren()

Money:Button("Banknote Farm",function()
    local children = game.Workspace:GetChildren()
    
    for _, child in pairs(children) do
    for _, child in pairs(child:GetChildren()) do
    end
    if child:IsA("Tool") and child.Name == "Banknote" then
        child.Handle.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
        wait(0.1)
        end
    end
end)

local BanknoteToggle = false
Money:Toggle("Banknote Farm",function(bool4)
BanknoteToggle = bool4
end)

spawn(function()
while wait() do
if BanknoteToggle then
    local children = game.Workspace:GetChildren()
    
    for _, child in pairs(children) do
    for _, child in pairs(child:GetChildren()) do
    end
    
    if child:IsA("Tool") and child.Name == "Banknote" then
        child.Handle.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
        wait(0.1)
        end
    end
end
end
end)
