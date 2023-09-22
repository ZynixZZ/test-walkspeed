-- This walkspeed script is the same as others , but does not change to default speed when you reset. ENJOY !    
_G.HackedWalkSpeed = 100
 
local Plrs = game:GetService("Players")
 
local MyPlr = Plrs.LocalPlayer
local MyChar = MyPlr.Character
 
if MyChar then
local Hum = MyChar.Humanoid
Hum.Changed:connect(function()
Hum.WalkSpeed = _G.HackedWalkSpeed
end)
Hum.WalkSpeed = _G.HackedWalkSpeed
end
 
 
MyPlr.CharacterAdded:connect(function(Char)
MyChar = Char
repeat wait() until Char:FindFirstChild("Humanoid")
local Hum = Char.Humanoid
Hum.Changed:connect(function()
Hum.WalkSpeed = _G.HackedWalkSpeed
end)
Hum.WalkSpeed = _G.HackedWalkSpeed
end)
 
-- end of script :)
