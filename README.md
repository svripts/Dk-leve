local ScreenGui = Instance.new("ScreenGui")
local Button = Instance.new("TextButton")
local Corner = Instance.new("UICorner")

local Player = game.Players.LocalPlayer

ScreenGui.Name = "DKHelp"
ScreenGui.Parent = Player:WaitForChild("PlayerGui")

Button.Parent = ScreenGui
Button.Size = UDim2.new(0, 100, 0, 100)
Button.Position = UDim2.new(0.9, -50, 0.1, -50)

Button.Text = "Sair"
Button.TextScaled = true
Button.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
Button.TextColor3 = Color3.fromRGB(255, 255, 255)

Corner.Parent = Button
Corner.CornerRadius = UDim.new(1, 0)

Button.MouseButton1Click:Connect(function()
	Player:Kick("Saindo do jogo...")
end)
