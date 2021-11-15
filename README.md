local erdaloyunda = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local erdal = Instance.new("TextButton")
local para = Instance.new("TextButton")
local ImageLabel = Instance.new("ImageLabel")
local ImageLabel_2 = Instance.new("ImageLabel")

--Properties:

erdaloyunda.Name = "erdaloyunda"
erdaloyunda.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
erdaloyunda.ResetOnSpawn = false

Frame.Parent = erdaloyunda
Frame.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Frame.Position = UDim2.new(0.190643281, 0, 0.182926834, 0)
Frame.Size = UDim2.new(0, 528, 0, 260)
Frame.Active = true
Frame.Draggable = true

erdal.Name = "erdal"
erdal.Parent = Frame
erdal.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
erdal.BackgroundTransparency = 0.200
erdal.Position = UDim2.new(0.407290041, 0, 0.156097591, 0)
erdal.Size = UDim2.new(0, 97, 0, 50)
erdal.Font = Enum.Font.SourceSans
erdal.Text = "Erdal Doc"
erdal.TextColor3 = Color3.fromRGB(255, 255, 255)
erdal.TextScaled = true
erdal.TextSize = 14.000
erdal.TextWrapped = true
erdal.MouseButton1Down:connect(function()
	_G.autoTap = false
	while _G.autoTap == true do
		local args = {
			[1] = "Block",
			[2] = true
		}

		game:GetService("ReplicatedStorage").MainEvent:FireServer(unpack(args))

		wait()
	end
end)

para.Name = "para"
para.Parent = Frame
para.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
para.Position = UDim2.new(0.197919995, 0, 0.582364023, 0)
para.Size = UDim2.new(0, 318, 0, 83)
para.Font = Enum.Font.SourceSans
para.Text = "Bas Parayı Abicim (10k)"
para.TextColor3 = Color3.fromRGB(255, 255, 255)
para.TextScaled = true
para.TextSize = 14.000
para.TextWrapped = true
para.MouseButton1Down:connect(function()
	_G.autoTap = false
	while _G.autoTap == true do
		local args = {
			[1] = "DropMoney",
			[2] = "10000"
		}

		game:GetService("ReplicatedStorage").MainEvent:FireServer(unpack(args))

		wait()
	end
end)

ImageLabel.Parent = Frame
ImageLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
ImageLabel.Position = UDim2.new(0.721929789, 0, 0.0642589033, 0)
ImageLabel.Size = UDim2.new(0, 131, 0, 98)
ImageLabel.Image = "rbxassetid://8007735447"

ImageLabel_2.Parent = Frame
ImageLabel_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
ImageLabel_2.Position = UDim2.new(0.0504319221, 0, 0.0681050569, 0)
ImageLabel_2.Size = UDim2.new(0, 131, 0, 98)
ImageLabel_2.Image = "rbxassetid://8007735447"
