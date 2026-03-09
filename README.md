# Vansuclocal Key = "kienvan36thanhhoa"

local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local TextBox = Instance.new("TextBox")
local Button = Instance.new("TextButton")

ScreenGui.Parent = game.CoreGui

Frame.Parent = ScreenGui
Frame.Size = UDim2.new(0,250,0,120)
Frame.Position = UDim2.new(0.5,-125,0.5,-60)
Frame.BackgroundColor3 = Color3.fromRGB(40,40,40)

TextBox.Parent = Frame
TextBox.Size = UDim2.new(0,200,0,30)
TextBox.Position = UDim2.new(0.5,-100,0.25,0)
TextBox.PlaceholderText = "Nhập key..."

Button.Parent = Frame
Button.Size = UDim2.new(0,200,0,30)
Button.Position = UDim2.new(0.5,-100,0.6,0)
Button.Text = "Xác nhận"

Button.MouseButton1Click:Connect(function()

if TextBox.Text == Key then

Frame:Destroy()

print("Key đúng, đang chạy script...")

loadstring(game:HttpGet("https://raw.githubusercontent.com/vaidhdhdgdhd/Vansuc/main/ki%E1%BA%BFn%20v%C4%83n%20hud%20v2.txt"))()

else

game.Players.LocalPlayer:Kick("Sai Key!")

end

end)
