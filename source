    local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("Vidaflare", "Ocean")
local Main = Window:NewTab("Main")
local Player = Window:NewTab("Player")
local Extra = Window:NewTab("Extra")
local PlayerSection = Player:NewSection("Local Player")
local ExtraSection = Extra:NewSection("Extra")
local PrisonSection = Main:NewSection("Prison Life")

--MAIN
PrisonSection:NewDropdown("Guns", "Gives you guns", {"Remington 870", "M9", "AK-47", }, function(v)
local A_1 = game:GetService("Workspace")["Prison_ITEMS"].giver[v].ITEMPICKUP
local Event = game:GetService("Workspace").Remote.ItemHandler
Event:InvokeServer(A_1)

    print(currentOption)
end)

PrisonSection:NewDropdown("Misc", "Other stuff (Key Card may not work cuz there needs to be one dropped.)", {"Crude Knife", "Hammer", "Key Card"}, function(V)
    local A_1 = game:GetService("Workspace")["Prison_ITEMS"].single[V].ITEMPICKUP
    local Event = game:GetService("Workspace").Remote.ItemHandler
    Event:InvokeServer(A_1)
    
        print(currentOption)
    end)

PrisonSection:NewButton("Infinite Yield", "basically admin", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source"))()
    print("Clicked")
end)





--EXTRA
ExtraSection:NewLabel("Made by sxn#8271")
ExtraSection:NewKeybind("Keybind", "Toggle UI", Enum.KeyCode.V, function()
	Library:ToggleUI()
end)


--PLAYER
PlayerSection:NewSlider("Walkspeed", "Changes walkspeed.", 500, 0, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)
PlayerSection:NewSlider("JumpPower", "Changes how high you can jump.", 500, 0, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.JumpPower = s
end)





