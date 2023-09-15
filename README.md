-- Made By iWasThisi
-- Instances:
local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local TextBox = Instance.new("TextBox")
local TextButton = Instance.new("TextButton")
--Properties:
 
ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
 
Frame.Parent = ScreenGui
Frame.BackgroundColor3 = Color3.new(1, 1, 1)
Frame.Position = UDim2.new(0.288659781, 0, 0.220588237, 0)
Frame.Size = UDim2.new(0, 148, 0, 83)
 
TextBox.Parent = ScreenGui
TextBox.BackgroundColor3 = Color3.new(1, 1, 1)
TextBox.Position = UDim2.new(0.300257713, 0, 0.235294089, 0)
TextBox.Size = UDim2.new(0, 129, 0, 30)
TextBox.Font = Enum.Font.SourceSans
TextBox.Text = "ENTER WALKSPEED"
TextBox.TextColor3 = Color3.new(0, 0, 0)
TextBox.TextSize = 14
 
TextButton.Parent = ScreenGui
TextButton.BackgroundColor3 = Color3.new(1, 1, 1)
TextButton.Position = UDim2.new(0.319587618, 0, 0.297385603, 0)
TextButton.Size = UDim2.new(0, 98, 0, 28)
TextButton.Font = Enum.Font.SourceSans
TextButton.Text = "Get WalkSpeed"
TextButton.TextColor3 = Color3.new(0, 0, 0)
TextButton.TextSize = 14
-- Scripts:
TextButton.MouseButton1Down:Connect(function()
	game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = TextBox.Text
end)
