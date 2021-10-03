local library = loadstring(game:HttpGet(('https://raw.githubusercontent.com/AikaV3rm/UiLib/master/Lib.lua')))()

local WizLeg = library:CreateWindow("Wizard Legends")
local Upgrade = WizLeg:CreateFolder("Upgrade")
local Eggs = WizLeg:CreateFolder("Eggs")
local Codes = WizLeg:CreateFolder("Codes")
local Other = WizLeg:CreateFolder("Other")
local Credits = WizLeg:CreateFolder("Credits")

-- Upgrade

Upgrade:Button("Upgrade Mind",function()
    game:GetService("ReplicatedStorage").UpgradeStatLevel:InvokeServer("BackpackLevel")
end)

Upgrade:Button("Upgrade Mind MAX",function()
    game:GetService("ReplicatedStorage").UpgradeAllStatLevel:InvokeServer("BackpackLevel")
end)

Upgrade:Button("Upgrade Wand",function()
    game:GetService("ReplicatedStorage").UpgradeStatLevel:InvokeServer("WandLevel")
end)

Upgrade:Button("Upgrade Wand MAX",function()
    game:GetService("ReplicatedStorage").UpgradeAllStatLevel:InvokeServer("WandLevel")
end)

Upgrade:Button("Upgrade Cloak",function()
    game:GetService("ReplicatedStorage").UpgradeStatLevel:InvokeServer("CloakLevel")
end)

Upgrade:Button("Upgrade Cloak MAX",function()
    game:GetService("ReplicatedStorage").UpgradeAllStatLevel:InvokeServer("CloakLevel")
end)

Upgrade:Button("Upgrade Crest",function()
    game:GetService("ReplicatedStorage").UpgradeStatLevel:InvokeServer("CollectorLevel")
end)

Upgrade:Button("Upgrade Crest MAX",function()
    game:GetService("ReplicatedStorage").UpgradeAllStatLevel:InvokeServer("CollectorLevel")
end)

Upgrade:Button("Rebirth",function()
    game:GetService("ReplicatedStorage").UpgradeStatLevel:InvokeServer("RankLevel")
end)

local mindtoggle = false
Upgrade:Toggle("Mind",function(bool5)
mindtoggle = bool5
end)

spawn(function()
while wait() do
if manatoggle then
    game:GetService("ReplicatedStorage").UpgradeAllStatLevel:InvokeServer("BackpackLevel")
end
end
end)

local wandtoggle = false
Upgrade:Toggle("Wand",function(bool6)
wandtoggle = bool6
end)

spawn(function()
while wait() do
if wandtoggle then
    game:GetService("ReplicatedStorage").UpgradeAllStatLevel:InvokeServer("WandLevel")
end
end
end)

local cloaktoggle = false
Upgrade:Toggle("Cloak",function(bool7)
cloaktoggle = bool7
end)

spawn(function()
while wait() do
if cloaktoggle then
    game:GetService("ReplicatedStorage").UpgradeAllStatLevel:InvokeServer("CloakLevel")
end
end
end)

local cresttoggle = false
Upgrade:Toggle("Crest",function(bool8)
cresttoggle = bool8
end)

spawn(function()
while wait() do
if cresttoggle then
    game:GetService("ReplicatedStorage").UpgradeAllStatLevel:InvokeServer("CollectorLevel")
end
end
end)

Eggs:Label("Area 1",Color3.fromRGB(38,38,38),Color3.fromRGB(0,216,111))

Eggs:Button("Rat Egg",function()
    game:GetService("ReplicatedStorage").PetStoreRoll:InvokeServer("VillageRatShop")
end)

Eggs:Button("Cat Egg",function()
    game:GetService("ReplicatedStorage").PetStoreRoll:InvokeServer("VillageCatShop")
end)

Eggs:Button("Piguel Egg",function()
    game:GetService("ReplicatedStorage").PetStoreRoll:InvokeServer("VillagePorkshop")
end)

local rateggtoggle = false
Eggs:Toggle("Rat Egg",function(bool1)
rateggtoggle = bool1
end)

spawn(function()
while wait() do
if rateggtoggle then
game:GetService("ReplicatedStorage").PetStoreRoll:InvokeServer("VillageRatShop")
end
end
end)

local categgtoggle
Eggs:Toggle("Cat Egg",function(bool2)
categgtoggle = bool2
end)

spawn(function()
while wait() do
if categgtoggle then
game:GetService("ReplicatedStorage").PetStoreRoll:InvokeServer("VillageCatShop")
end
end
end)

local pigueleggtoggle
Eggs:Toggle("Piguel Egg",function(bool3)
pigueleggtoggle = bool3
end)

spawn(function()
while wait() do
if pigueleggtoggle then
game:GetService("ReplicatedStorage").PetStoreRoll:InvokeServer("VillagePorkshop")
end
end
end)

Eggs:Label("Area 2",Color3.fromRGB(38,38,38),Color3.fromRGB(0,216,111))

Codes:Button("Use all codes",function()
    game:GetService("ReplicatedStorage").PromoCodeRequest:InvokeServer("magicalcodes")
    game:GetService("ReplicatedStorage").PromoCodeRequest:InvokeServer("potofgold")
    game:GetService("ReplicatedStorage").PromoCodeRequest:InvokeServer("manaparty")
    game:GetService("ReplicatedStorage").PromoCodeRequest:InvokeServer("PlanetMilo")
    game:GetService("ReplicatedStorage").PromoCodeRequest:InvokeServer("dragon")
    game:GetService("ReplicatedStorage").PromoCodeRequest:InvokeServer("snuglife")
    game:GetService("ReplicatedStorage").PromoCodeRequest:InvokeServer("youtubemana")
    game:GetService("ReplicatedStorage").PromoCodeRequest:InvokeServer("youtubewizard")
    game:GetService("ReplicatedStorage").PromoCodeRequest:InvokeServer("wizardlegends")
    game:GetService("ReplicatedStorage").PromoCodeRequest:InvokeServer("magiccoins")
end)

-- Other

Other:Button("Tp to sell",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").World["City Island"].Village.SellShop.Hoop.Collider.CFrame
end)

Other:Button("   Tp all mana to you",function()
    local children = workspace.MouseFiltered.ManaSpawners.Village:GetChildren()
        for _, child in pairs(children) do
        for _, child in pairs(child:GetChildren()) do
    end
    if child:IsA("BasePart") and child.Name == "Mana" then
        child.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
    end
    end
end)

Credits:Label("Made by Prudin#6667",Color3.fromRGB(38,38,38),Color3.fromRGB(0,216,111))
