-- Only works for M9

local library = loadstring(game:HttpGet(('https://raw.githubusercontent.com/AikaV3rm/UiLib/master/Lib.lua')))()

local PrisonLife = library:CreateWindow("Prison Life")
local Guns = PrisonLife:CreateFolder("Guns")
local gun = game.Workspace.Prison_ITEMS.giver:GetChildren()
local inf = 999999999999999999999999999999999999999999999999999999999999999999999

Guns:Button("Infinite Ammo",function()
    MaxAmmoM9 = require(game.Players.LocalPlayer.Backpack.M9.GunStates)
    MaxAmmoM9.MaxAmmo = inf
    CurrentAmmoM9 = require(game.Players.LocalPlayer.Backpack.M9.GunStates)
    CurrentAmmoM9.CurrentAmmo = inf
    Spread = require(game.Players.LocalPlayer.Backpack.M9.GunStates)
    Spread.Spread.Min = 0
    Spread.Spread.Max = 0
end)
