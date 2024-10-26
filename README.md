local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("GUL HUB Survive in area 51 | Beta v1 ", "DarkTheme")

--Script

local Welcom = Window:NewTab("Welcom")
local WelcomSection = Welcom:NewSection("By mm55061 | 4737901580")
local WelcomSection = Welcom:NewSection("Map Survive in area 51 | 2214661900")

local Main = Window:NewTab("Main")
local MainSection = Main:NewSection("Clicked to Tp")
MainSection:NewButton("Spawn", "", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(630.1624145507812, 1148.4998779296875, 749.1951293945312) --Spawn
end)
MainSection:NewButton("Shop", "", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(589.678955078125, 1150.9998779296875, 664.4775390625) --Shop
end)
MainSection:NewButton("Crafting Room", "", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(953.6991577148438, 1059.9998779296875, 714.219482421875) --Crafting Room
end)
MainSection:NewButton("Portal", "", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-108.6634521484375, 981.9999389648438, 797.7275390625) --Portal
end)
MainSection:NewButton("Metro Station", "", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-492.34515380859375, 916.1000366210938, -57.4563102722168) --Metro Station
end)
local Gun = Window:NewTab("Gun")
local GunSection = Gun:NewSection("Clicked to Tp")
GunSection:NewButton("ice crossbow", "", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(242.7141876220703, 699.3610229492188, 943.5986328125) --ice crossbow
end)
GunSection:NewButton("Vulcan", "", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-600.4874877929688, 957.235595703125, 155.46588134765625) --Vulcan
end)
GunSection:NewButton("Red Missile Launcher", "", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-353.5192565917969, 1072.9974365234375, 411.0243835449219) --Red Missile Launcher
end)
GunSection:NewButton("LXW", "", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-15.062729835510254, 860.9974975585938, -46.453834533691406) --LXW
end)

--Open and close Gui

local ScreenGui = Instance.new("ScreenGui")
ScreenGui.Name = "ScreenGui"
ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
ScreenGui.ResetOnSpawn = false
 
local Toggle = Instance.new("TextButton")
Toggle.Name = "Toggle"
Toggle.Parent = ScreenGui
Toggle.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Toggle.Position = UDim2.new(0, 0, 0.454706937, 0)
Toggle.Size = UDim2.new(0, 90, 0, 38)
Toggle.Font = Enum.Font.SourceSans
Toggle.Text = "Open"
Toggle.TextColor3 = Color3.fromRGB(248, 248, 248)
Toggle.TextSize = 28.000
Toggle.Draggable = true
Toggle.MouseButton1Click:connect(function()
    Library:ToggleUI()
end)
 
local Corner = Instance.new("UICorner")
Corner.Name = "Corner"
Corner.Parent = Toggle
