local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("ไอ่เซนHub Version:0.2.4", "Synapse")
--Credit
local Tab = Window:NewTab("Credit")
local Section = Tab:NewSection("Owner:ไอ่เซน or WhiteCat#3858")
local Section = Tab:NewSection("Tester:ไอ่ชิน or floppa gaming#3445")

----changelogs
local Tab = Window:NewTab("Changelogs")
local Section = Tab:NewSection("BETA Auto Farm")
local Section = Tab:NewSection("")
local Section = Tab:NewSection("")
local Section = Tab:NewSection("")
local Section = Tab:NewSection("")
---------Teleport
local Tab = Window:NewTab("Teleport")
local Section = Tab:NewSection("TEAM TELEPORT")
Section:NewButton("Red Team", "YOU WILL TELEPORT TO RED TEAM OK??แล้วก็ made by ไอ่เซน ", function()
    
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(482.994324, -6.38043165, -64.6908035, -0.0168182235, -0.0869451985, 0.9960711, -7.61250796e-09, 0.996212006, 0.0869574994, -0.999858558, 0.00146246306, -0.0167545173)

    

end)
Section:NewButton("White Team", "YOU WILL TELEPORT TO WHITE TEAM OK??แล้วก็ made by ไอ่เซน", function()
    
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-50.5733147, -4.6061511, -607.829224, -0.99955219, -0.00234889495, 0.0298310202, -8.02267142e-09, 0.996914387, 0.078496784, -0.0299233533, 0.0784616321, -0.996467948)


end)
Section:NewButton("Black Team", "YOU WILL TELEPORT TO BLACK TEAM OK??แล้วก็ made by ไอ่เซน", function()
    
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-590.467896, -6.18136215, -69.4435654, 0.0205775853, 0.0970736817, -0.995064437, -6.60664812e-09, 0.995275199, 0.0970942378, 0.999788284, -0.0019979584, 0.0204803608)


end)

Section:NewButton("Green Team", "YOU WILL TELEPORT TO GREEN TEAM OK??แล้วก็ made by ไอ่เซน", function()
    
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-590.172424, -3.98905802, 294.95871, 0.0047372859, 0.147594064, -0.989036679, 7.09072667e-09, 0.989047766, 0.147595719, 0.999988794, -0.000699210097, 0.00468540099)
    
end)

Section:NewButton("Purple Team", "YOU WILL TELEPORT TO PURPLE TEAM OK???แล้วก็ made by ไอ่เซน", function()
    
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(481.588379, -4.90746498, 647.344482, -0.0635458902, -0.0597306043, 0.996189833, 8.06757683e-09, 0.998207271, 0.0598515719, -0.997978926, 0.00380332931, -0.0634319708)

end)

Section:NewButton("Yellow Team", "YOU WILL TELEPORT TO YELLOW TEAM OKIE?แล้วก้ made by ไอ่เซน", function()
  
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-593.528625, -0.588476181, 639.921265, 0.0095742913, 0.103795618, -0.994552553, 8.69098571e-09, 0.99459815, 0.103800379, 0.999954164, -0.000993823633, 0.00952257123)

end)
Section:NewButton("Blue Team", "YOU WILL TELEPORT TO YELLOW TEAM OK?", function()
    
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(484.0625, -5.28055716, 299.01712, 0.123323344, -0.126441061, 0.98427844, 4.06751344e-09, 0.991849661, 0.12741366, -0.992366552, -0.0157130752, 0.122318216)
end)
local Section = Tab:NewSection("Teleport Player")
Plr = {}
for i,v in pairs(game:GetService("Players"):GetChildren()) do 
    table.insert(Plr,v.Name)
end    
local drop = Section:NewDropdown("Select Player", "Click to Select", Plr, function(t)
    PlayerTP = t
end)
Section:NewButton("Teleport", "it just teleport;-;", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players[PlayerTP].Character.HumanoidRootPart.CFrame
end)
    Section:NewToggle("Auto Teleport", "Press to auto Teleport", function(t)
    _G.TeleportPlayer = t 
    while _G.TeleportPlayer do wait()        
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players[PlayerTP].Character.HumanoidRootPart.CFrame
    end
    end)

  Section:NewButton("Refresh Player*NOTWORK SO DONT USE IT*", "Click to Refresh", function()
    drop:Refresh(Plr)
  end)
  local Tab = Window:NewTab("AutoFarm*BETA*")
local Section = Tab:NewSection("AutoFarm*BETA VERSION*")
Section:NewToggle("Auto-Farm", "On-Off Auto-Farm", function()
   game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-70.642746, 153.013443, 580.171936, -0.997024596, -0.00670335628, 0.0767921731, -8.65865601e-09, 0.996211708, 0.0869613737, -0.0770841911, 0.0867026299, -0.993247569)
    wait(0.1)
   local TweenService = game:GetService("TweenService")
 local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(20, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(-56.4987564, 50.6605911, 9463.18555, -0.106840596, -0.878039002, 0.466511071, -1.64060783e-08, 0.469196677, 0.883093715, -0.994276166, 0.0943502486, -0.0501292646)}):Play()
wait(20) 
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-55.6248283, -356.100067, 9494.95508, -0.997524858, -3.1820381e-08, 0.0703145266, -2.92097724e-08, 1, 3.81558252e-08, -0.0703145266, 3.60075134e-08, -0.997524858)
    wait(0.1)
end)
