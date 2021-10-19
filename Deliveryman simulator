local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/GreenDeno/Venyx-UI-Library/main/source.lua"))()
local venyx = library.new("Deliveryman Simulator", 5013109572)

local themes = {
Background = Color3.fromRGB(24, 24, 24),
Glow = Color3.fromRGB(0, 0, 0),
Accent = Color3.fromRGB(10, 10, 10),
LightContrast = Color3.fromRGB(20, 20, 20),
DarkContrast = Color3.fromRGB(14, 14, 14),  
TextColor = Color3.fromRGB(255, 255, 255)
}

local deliverItemDelay = 2.6
local selectedArea;
local selectedStrength;
local selectedItem;
local selectedItemLocation;
local itemAmount;

local energyCount = game.Players.LocalPlayer.leaderstats.Energy.Value
local strengthCount = game.Players.LocalPlayer.leaderstats.Strength.Value

local function findArea(item)
    if item == "Small Box (1 Strength)" then
        selectedArea = "Beach"
    elseif item == "Box (5 Strength)" then
        selectedArea = "Beach"
    elseif item == "Large Box (25 Strength)" then
        selectedArea = "Beach"
    elseif item == "Golden Chest (50 Strength)" then
        selectedArea = "Event"
    elseif item == "Shiny Box (66.6 Strength)" then
        selectedArea = "Beach"
    elseif item == "Golden Box (200 Strength)" then
        selectedArea = "Beach"
    elseif item == "Plate (416 Strength)" then
        selectedArea = "Winter"
    elseif item == "Ruby Chest (500 Strength)" then
        selectedArea = "Event"
    elseif item == "Lantern (900 Strength)" then
        selectedArea = "Winter"
    elseif item == "Rock (1.5k Strength)" then
        selectedArea = "Winter"
    elseif item == "Seat (3.5k Strength)" then
        selectedArea = "Winter"
    elseif item == "Log (5k Strength)" then
        selectedArea = "Winter"
    elseif item == "Golf Ball (6.6k Strength)" then
        selectedArea = "City"
    elseif item == "Diamond Chest (10k Strength)" then
        selectedArea = "Event"
    elseif item == "Pool Ball (11k Strength)" then
        selectedArea = "City"
    elseif item == "Basketball (14k Strength)" then
        selectedArea = "City"
    elseif item == "Pillow (18k Strength)" then
        selectedArea = "City"
    elseif item == "Ice (22.5k Strength)" then
        selectedArea = "City"
    elseif item == "Emerald Chest (25k Strength)" then
        selectedArea = "Event"
    elseif item == "Bread (41.6k Strength)" then
        selectedArea = "Atlantis"
    elseif item == "Sodalite Chest (60k Strength)" then
        selectedArea = "Event"
    elseif item == "Book (65k Strength)" then
        selectedArea = "Atlantis"
    elseif item == "Saw (75k Strength)" then
        selectedArea = "Atlantis"
    elseif item == "Stappy (100k Strength)" then
        selectedArea = "Atlantis"
    elseif item == "Cake (120k Strength)" then
        selectedArea = "Atlantis"
    elseif item == "Fries (150k Strength)" then
        selectedArea = "Moon"
    elseif item == "Remote (220k Strength)" then
        selectedArea = "Moon"
    elseif item == "Crate (300k Strength)" then
        selectedArea = "Moon"
    elseif item == "Barrel (370k Strength)" then
        selectedArea = "Moon"
    elseif item == "Rowboat (450k Strength)" then
        selectedArea = "Moon"
    elseif item == "Mushroom (560k Strength)" then
        selectedArea = "Candy"
    elseif item == "Crystal (825k Strength)" then
        selectedArea = "Candy"
    elseif item == "Cart (1M Strength)" then
        selectedArea = "Candy"
    elseif item == "Fountain (1.35M Strength" then
        selectedArea = "Candy"
    elseif item == "Cobble Wall (1.65M Strength)" then
        selectedArea = "Candy"
    elseif item == "Steak Uncooked (2.25M Strength)" then
        selectedArea = "Cherry"
    elseif item == "Burger (2.6M Strength)" then
        selectedArea = "Cherry"
    elseif item == "Shrimp (3M Strength)" then
        selectedArea = "Cherry"
    elseif item == "Watermelon (3.5M Strength)" then
        selectedArea = "Cherry"
    elseif item == "Toast (4.1M Strength)" then
        selectedArea = "Cherry"
    elseif item == "Muffin (8.35M Strength)" then
        selectedArea = "Cherry"
    elseif item == "Sweet Pepper (11M Strength)" then
        selectedArea = "Cherry"
    elseif item ==  "Hotdog (15M Strength)" then
        selectedArea = "Cherry"
    elseif item == "Cube (24M Strength)" then
        selectedArea = "Volcano"
    elseif item == "Colors Cube (30M Strength)" then
        selectedArea = "Volcano"
    elseif item == "Heart Cube (45M Strength)" then
        selectedArea = "Volcano"
    elseif item == "Dark Matter (65M Strength)" then
        selectedArea = "Volcano"
    elseif item == "Ice Cube (90M Strength)" then
        selectedArea = "Volcano"
    end
end

local function pickup(amount)
    repeat
        keypress(0x45)
        wait(0.01)
        keyrelease(0x45)
        amount = amount - 1
    until amount == 0
end

local function train()
    keypress(0x45)
    wait(0.5)
    keyrelease(0x45)
end

--main page
local page = venyx:addPage("Main", 5012544693)
local section1 = page:addSection("Teleport")
local section2 = page:addSection("Autofarm")
local section3 = page:addSection("Other")

--section 1
section1:addDropdown("Areas", {"Beach", "Winter", "City", "Atlantis", "Moon", "Candy", "Cherry", "Skull", "Volcano", "Event"}, function(option)
    if option == "Beach" then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-113, 4, -223)
    elseif option == "Winter" then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-111, 4, -61)
    elseif option == "City" then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-111, 4, 108)
    elseif option == "Atlantis" then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-111, 4, 283)
    elseif option == "Moon" then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-111, 4, 454)
    elseif option == "Candy" then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-111, 4, 621)
    elseif option == "Cherry" then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(636, -21, 26)
    elseif option == "Skull" then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1577, 263, -42)
    elseif option == "Volcano" then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-111, 4, 783)
    elseif option == "Event" then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-454, 4, -50)
    end
end)

section1:addDropdown("Training", {"Normal Strength", "1x Strength", "2x Strength", "3x Strength", "4x Strength", "25x Strength", "35x Strength"}, function(option)
    if option == "Normal Strength" then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-75, 5, -287)
    elseif option == "1x Strength" then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-72, 4, 130)
    elseif option == "2x Strength" then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-72, 4, 287)
    elseif option == "3x Strength" then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-72, 4, 455)
    elseif option == "4x Strength" then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-72, 4, 633)
    elseif option == "25x Strength" then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-84, 4, 1002)
    elseif option == "35x Strength" then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-524, 4, 5)
    end
end)

--section 2
local autofarmToggle;
section2:addToggle("Autofarm", false, function(bool)
    autofarmToggle = bool
end)

spawn(function()
    while wait() do
        if autofarmToggle then
            -- Starting
            print("Autofarming")
            
            wait(0.5)

            -- Find and teleport to selected item
            if selectedItem == "Small Box (1 Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-159, 5, -194) -- The begin of a hurtful journey because if stupid and can't code (Basically yandere dev coding rn)
            elseif selectedItem == "Box (5 Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-135, 7, -195)
            elseif selectedItem == "Large Box (25 Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-108, 9, -195)
            elseif selectedItem == "Golden Chest (50 Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-504, 9, -21)
            elseif selectedItem == "Shiny Box (66 Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-85, 7, -194)
            elseif selectedItem == "Golden Box (200 Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-59, 9, -195)
            elseif selectedItem == "Plate (416 Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-160, 4, -25)
            elseif selectedItem == "Ruby Chest (500 Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-479, 4, -16)
            elseif selectedItem == "Lantern (900 Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-135, 6, -28)
            elseif selectedItem == "Rock (1.5k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-109, 7, -27)
            elseif selectedItem == "Seat (3.5k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-83, 6, -28)
            elseif selectedItem == "Log (5k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-59, 6, -27)
            elseif selectedItem == "Golf Ball (6.6k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-160, 7, 143)
            elseif selectedItem == "Diamond Chest (10k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-452, 4, -16)
            elseif selectedItem == "Pool Ball (11k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-133, 8, 143)
            elseif selectedItem == "Basketball (14k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-109, 9, 143)
            elseif selectedItem == "Pillow (18k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-84, 7, 143)
            elseif selectedItem == "Ice (22.5k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-58, 6, 143)
            elseif selectedItem == "Emerald Chest (25k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-429, 4, -16)
            elseif selectedItem == "Bread (41.6k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-159, 5, 312)
            elseif selectedItem ==  "Sodalite Chest (60k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-403, 4, -15)
            elseif selectedItem == "Book (65k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-134, 5, 312)
            elseif selectedItem == "Saw (75k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-109, 5, 312)
            elseif selectedItem == "Stappy (100k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-84, 8, 312)
            elseif selectedItem == "Cake (120k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-60, 8, 312)
            elseif selectedItem == "Fries (150k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-159, 6, 480)
            elseif selectedItem == "Remote (220k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-133, 5, 480)
            elseif selectedItem == "Crate (300k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-109, 9, 482)
            elseif selectedItem == "Barrel (370k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-84, 4, 485)
            elseif selectedItem == "Rowboat (450k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-59, 7, 482)
            elseif selectedItem == "Mushroom (560k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-160, 9, 650)
            elseif selectedItem == "Crystal (825k Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-134, 8, 650)
            elseif selectedItem == "Cart (1M Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-109, 6, 650)
            elseif selectedItem == "Fountain (1.35M Strength" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-83, 9, 650)
            elseif selectedItem == "Cobble Wall (1.65M Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-59, 9, 650)
            elseif selectedItem == "Steak Uncooked (2.25M Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(644, -20, 59)
            elseif selectedItem == "Burger (2.6M Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(702, -21, 79)
            elseif selectedItem == "Shrimp (3M Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(760, -21, 57)
            elseif selectedItem == "Watermelon (3.5M Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(784, -21, 0)
            elseif selectedItem == "Toast (4.1M Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(763, -19, -60)
            elseif selectedItem == "Muffin (8.35M Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(705, -21, -81)
            elseif selectedItem == "Sweet Pepper (11M Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(646, -21, -58)
            elseif selectedItem == "Hotdog (15M Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(622, -21, 1)
            elseif selectedItem == "Cube (24M Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-160, 4, 807)
            elseif selectedItem == "Colors Cube (30M Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-134, 4, 807)
            elseif selectedItem == "Heart Cube (45M Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-109, 4, 807)
            elseif selectedItem == "Dark Matter (65M Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-84, 4, 807)
            elseif selectedItem == "Ice Cube (90M Strength)" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-59, 4, 807)
            end
            wait(1.3) -- Delay so you always pick up the item
            pickup(itemAmount) -- Pickup amount
            wait(deliverItemDelay) -- Wait .. Seconds
            findArea(selectedItem)
            if selectedArea == "Beach" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-109, 4, -132) -- Teleport To The Finish Line
            elseif selectedArea == "Winter" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-109, 4, 38) -- Teleport To The Finish Line
            elseif selectedArea == "City" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-109, 4, 206) -- Teleport To The Finish Line
            elseif selectedArea == "Atlantis" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-109, 4, 376) -- Teleport To The Finish Line
            elseif selectedArea == "Moon" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-109, 4, 542) -- Teleport To The Finish Line
            elseif selectedArea == "Candy" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-109, 4, 713) -- Teleport To The Finish Line
            elseif selectedArea == "Cherry" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(683, -20, 19) -- Teleport To The Finish Line
            elseif selectedArea == "Event" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-455, 4, 37)
            elseif selectedArea == "Volcano" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-97, 4, 975)
            end
        end
    end
end)

section2:addDropdown("Item", {"Small Box (1 Strength)", "Box (5 Strength)", "Large Box (25 Strength)", "Golden Chest (50 Strength)", "Shiny Box (66.6 Strength)", "Golden Box (200 Strength)", "Plate (416 Strength)", "Ruby Chest (500 Strength)", "Lantern (900 Strength)", "Rock (1.5k Strength)", "Seat (3.5k Strength)", "Log (5k Strength)", "Golf Ball (6.6k Strength)", "Diamond Chest (10k Strength)", "Pool Ball (11k Strength)", "Basketball (14k Strength)", "Pillow (18k Strength)", "Ice (22.5k Strength)", "Emerald Chest (25k Strength)", "Bread (41.6k Strength)", "Sodalite Chest (60k Strength)", "Book (65k Strength)", "Saw (75k Strength)", "Stappy (100k Strength)", "Cake (120k Strength)", "Fries (150k Strength)", "Remote (220k Strength)", "Crate (300k Strength)", "Barrel (370k Strength)", "Rowboat (450k Strength)", "Mushroom (560k Strength)", "Crystal (825k Strength)", "Cart (1M Strength)", "Fountain (1.35M Strength", "Cobble Wall (1.65M Strength)", "Steak Uncooked (2.25M Strength)", "Burger (2.6M Strength)", "Shrimp (3M Strength)", "Watermelon (3.5M Strength)", "Toast (4.1M Strength)", "Muffin (8.35M Strength)", "Sweet Pepper (11M Strength)", "Hotdog (15M Strength)", "Cube (24M Strength)", "Colors Cube (30M Strength)", "Heart Cube (45M Strength)", "Dark Matter (65M Strength)", "Ice Cube (90M Strength)"}, function(option)
    selectedItem = option
    print("Selected Item: "..selectedItem)
end)

section2:addDropdown("Amount of items", {"1", "2", "3"}, function(option)
    if option == "1" then
        itemAmount = 1
    elseif option == "2" then
        itemAmount = 2
    elseif option == "3" then
        itemAmount = 3
    end
    print("Selected: "..option.." item/items")
end)

--section 3
section3:addButton("Train at normal", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-39, 5, -303)
    wait(0.25)
    train()
end)

section3:addButton("Train at 1x Strength", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-57, 4, 114)
    wait(0.25)
    train()
end)

section3:addButton("Train at 2x Strength", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-56, 4, 273)
    wait(0.25)
    train()
end)

section3:addButton("Train at 3x Strength", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-56, 4, 441)
    wait(0.25)
    train()
end)

section3:addButton("Train at 4x Strength", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-54, 4, 618)
    wait(0.25)
    train()
end)

section3:addButton("Train at 25x Strength", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-60, 4, 1017)
    wait(0.25)
    train()
end)

section3:addButton("Train at 35x Strength", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-533, 4, 34)
    wait(0.25)
    train()
end)

-- second page
local theme = venyx:addPage("Theme", 5012544693)
local colors = theme:addSection("Colors")

for theme, color in pairs(themes) do -- all in one theme changer, i know, im cool
    colors:addColorPicker(theme, color, function(color3)
        venyx:setTheme(theme, color3)
    end)
end

-- third page
local misc = venyx:addPage("Misc", 5012544693)
local libThings = misc:addSection("GUI Stuff")

libThings:addKeybind("Toggle Keybind", Enum.KeyCode.LeftControl, function()
    print("Activated Keybind")
    venyx:toggle()
end, function()
    print("Changed Keybind")
end)

-- load
venyx:SelectPage(venyx.pages[1], true)
