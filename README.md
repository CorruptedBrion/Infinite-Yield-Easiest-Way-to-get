-- Gui to Lua
-- Version: 3.2

-- Instances:

local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local UICorner = Instance.new("UICorner")
local Frame_2 = Instance.new("Frame")
local UICorner_2 = Instance.new("UICorner")
local TextLabel = Instance.new("TextLabel")
local Frame_3 = Instance.new("Frame")
local UICorner_3 = Instance.new("UICorner")
local TextLabel_2 = Instance.new("TextLabel")
local TextButton = Instance.new("TextButton")

--Properties:

ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
ScreenGui.ResetOnSpawn = false

Frame.Parent = ScreenGui
Frame.BackgroundColor3 = Color3.fromRGB(163, 42, 179)
Frame.Position = UDim2.new(0.0143884886, 0, 0.258010119, 0)
Frame.Size = UDim2.new(0, 257, 0, 286)
Frame.Active = true
Frame.Draggable = true

UICorner.Parent = Frame

Frame_2.Parent = Frame
Frame_2.BackgroundColor3 = Color3.fromRGB(87, 28, 89)
Frame_2.Size = UDim2.new(0, 257, 0, 48)

UICorner_2.CornerRadius = UDim.new(0, 3)
UICorner_2.Parent = Frame_2

TextLabel.Parent = Frame_2
TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.BackgroundTransparency = 1.000
TextLabel.Size = UDim2.new(0, 257, 0, 50)
TextLabel.Font = Enum.Font.SourceSans
TextLabel.Text = "Infinite Yield GUI"
TextLabel.TextColor3 = Color3.fromRGB(0, 0, 0)
TextLabel.TextScaled = true
TextLabel.TextSize = 14.000
TextLabel.TextWrapped = true

Frame_3.Parent = Frame
Frame_3.BackgroundColor3 = Color3.fromRGB(87, 28, 89)
Frame_3.Position = UDim2.new(0, 0, 0.832167804, 0)
Frame_3.Size = UDim2.new(0, 257, 0, 48)

UICorner_3.CornerRadius = UDim.new(0, 3)
UICorner_3.Parent = Frame_3

TextLabel_2.Parent = Frame_3
TextLabel_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel_2.BackgroundTransparency = 1.000
TextLabel_2.Size = UDim2.new(0, 257, 0, 50)
TextLabel_2.Font = Enum.Font.SourceSans
TextLabel_2.Text = "Made By CorruptedBrion on Youtube"
TextLabel_2.TextColor3 = Color3.fromRGB(0, 0, 0)
TextLabel_2.TextScaled = true
TextLabel_2.TextSize = 14.000
TextLabel_2.TextWrapped = true

TextButton.Parent = Frame
TextButton.BackgroundColor3 = Color3.fromRGB(75, 30, 107)
TextButton.Position = UDim2.new(0.0505836569, 0, 0.185314685, 0)
TextButton.Size = UDim2.new(0, 230, 0, 180)
TextButton.Font = Enum.Font.SourceSans
TextButton.Text = "Activate!"
TextButton.TextColor3 = Color3.fromRGB(0, 0, 0)
TextButton.TextScaled = true
TextButton.TextSize = 14.000
TextButton.TextWrapped = true
TextButton.MouseButton1Click:Connect(function()
	TextButton.Text="Enabling AntiBan..."
	wait(1)
	TextButton.Text="Executing in 3 Seconds!"
	wait(1)
	loadstring(game:HttpGet(('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'),true))()
	wait(1)
	TextButton.Text="Thanks For Using Our Script, - CorruptedBrion"
end)
