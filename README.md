-- Tạo GUI Menu cho Miku Hub
local menu = Instance.new("ScreenGui")
menu.Parent = game.Players.LocalPlayer.PlayerGui
menu.Name = "MikuHubMenu"

-- Tạo Frame cho Menu
local frame = Instance.new("Frame")
frame.Parent = menu
frame.Size = UDim2.new(0, 300, 0, 600)
frame.Position = UDim2.new(0, 10, 0, 10)
frame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
frame.BackgroundTransparency = 0.5

-- Tạo các nút trong menu
local buttonFarm = Instance.new("TextButton")
buttonFarm.Parent = frame
buttonFarm.Size = UDim2.new(0, 280, 0, 50)
buttonFarm.Position = UDim2.new(0, 10, 0, 10)
buttonFarm.Text = "Start Auto Farm"
buttonFarm.BackgroundColor3 = Color3.fromRGB(0, 255, 0)

local buttonRaid = Instance.new("TextButton")
buttonRaid.Parent = frame
buttonRaid.Size = UDim2.new(0, 280, 0, 50)
buttonRaid.Position = UDim2.new(0, 10, 0, 70)
buttonRaid.Text = "Start Auto Raid"
buttonRaid.BackgroundColor3 = Color3.fromRGB(255, 0, 0)

local buttonTP = Instance.new("TextButton")
buttonTP.Parent = frame
buttonTP.Size = UDim2.new(0, 280, 0, 50)
buttonTP.Position = UDim2.new(0, 10, 0, 130)
buttonTP.Text = "Teleport to Player"
buttonTP.BackgroundColor3 = Color3.fromRGB(0, 0, 255)

local buttonMastery = Instance.new("TextButton")
buttonMastery.Parent = frame
buttonMastery.Size = UDim2.new(0, 280, 0, 50)
buttonMastery.Position = UDim2.new(0, 10, 0, 190)
buttonMastery.Text = "Farm Mastery"
buttonMastery.BackgroundColor3 = Color3.fromRGB(255, 255, 0)

local buttonHaki = Instance.new("TextButton")
buttonHaki.Parent = frame
buttonHaki.Size = UDim2.new(0, 280, 0, 50)
buttonHaki.Position = UDim2.new(0, 10, 0, 250)
buttonHaki.Text = "Activate Haki"
buttonHaki.BackgroundColor3 = Color3.fromRGB(255, 165, 0)

local buttonSaber = Instance.new("TextButton")
buttonSaber.Parent = frame
buttonSaber.Size = UDim2.new(0, 280, 0, 50)
buttonSaber.Position = UDim2.new(0, 10, 0, 310)
buttonSaber.Text = "Auto Saber"
buttonSaber.BackgroundColor3 = Color3.fromRGB(128, 0, 128)

local buttonShop = Instance.new("TextButton")
buttonShop.Parent = frame
buttonShop.Size = UDim2.new(0, 280, 0, 50)
buttonShop.Position = UDim2.new(0, 10, 0, 370)
buttonShop.Text = "Auto Shop"
buttonShop.BackgroundColor3 = Color3.fromRGB(0, 255, 255)

-- Hàm xử lý Auto Farm
buttonFarm.MouseButton1Click:Connect(function()
    print("Auto Farm Started")
    -- Thêm mã Auto Farm vào đây
end)

-- Hàm xử lý Auto Raid
buttonRaid.MouseButton1Click:Connect(function()
    print("Auto Raid Started")
    -- Thêm mã Auto Raid vào đây
end)

-- Hàm xử lý Teleport to Player
buttonTP.MouseButton1Click:Connect(function()
    local playerToTP = game.Players:FindFirstChild("PlayerName") -- Thay 'PlayerName' bằng tên người chơi muốn TP
    if playerToTP then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = playerToTP.Character.HumanoidRootPart.CFrame
        print("Teleported to player: " .. playerToTP.Name)
    else
        print("Player not found.")
    end
end)

-- Hàm xử lý Farm Mastery
buttonMastery.MouseButton1Click:Connect(function()
    print("Starting Mastery Farm")
    -- Thêm mã Farm Mastery vào đây
end)

-- Hàm xử lý Haki
buttonHaki.MouseButton1Click:Connect(function()
    print("Activating Haki")
    -- Thêm mã kích hoạt Haki vào đây
end)

-- Hàm xử lý Auto Saber
buttonSaber.MouseButton1Click:Connect(function()
    print("Auto Saber Started")
    -- Thêm mã Auto Saber vào đây
end)

-- Hàm xử lý Auto Shop
buttonShop.MouseButton1Click:Connect(function()
    print("Auto Shop Started")
    -- Thêm mã Auto Shop vào đây
end)
