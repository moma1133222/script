--only skid if u give credit :3

local Rayfield = loadstring(game:HttpGet('https://sirius.menu/rayfield'))()

local Window = Rayfield:CreateWindow({
    Name = "moma hub",
    Icon = 0,
    LoadingTitle = "moma hub loading",
    LoadingSubtitle = "by moma1133222",
    Theme = "Default",
    DisableRayfieldPrompts = false,
    DisableBuildWarnings = false,
    ConfigurationSaving = {
       Enabled = false,
       FolderName = nil,
       FileName = "moma hub"
    },
    Discord = {
       Enabled = false,
       Invite = "noinvitelink",
       RememberJoins = true
    },
    KeySystem = false,
    KeySettings = {
       Title = "Untitled",
       Subtitle = "Key System",
       Note = "No method of obtaining the key is provided",
       FileName = "Key",
       SaveKey = true,
       GrabKeyFromSite = false,
       Key = {"Hello"}
    }
})

local Tab = Window:CreateTab("Main", 4483362458)
local Section = Tab:CreateSection("Main stuff")

Rayfield:Notify({
    Title = "Follow me please",
    Content = "my script blox moma1133222",
    Duration = 6.5,
    Image = 4483362458,
})

local ReplicatedStorage = game:GetService("ReplicatedStorage")
local remote = ReplicatedStorage:WaitForChild("Remotes"):WaitForChild("ClaimReward")

local args = {
    [1] = "Power",
    [2] = 0
}

local Input = Tab:CreateInput({
    Name = "Give Power(dont go to high or u WILL get kickt)",
    CurrentValue = "",
    PlaceholderText = "Give Power",
    RemoveTextAfterFocusLost = false,
    Flag = "Input1",
    Callback = function(Text)
        args[2] = tonumber(Text) or 300000000
        print("Input updated to:", args[2])
        remote:FireServer(unpack(args))
    end,
})

remote:FireServer(unpack(args))

local remote = ReplicatedStorage:WaitForChild("Remotes"):WaitForChild("Rebirth")

local args = {
    [1] = 0
}

local Input = Tab:CreateInput({
    Name = "Give Rebirths(max 1m)",
    CurrentValue = "",
    PlaceholderText = "Give rebirths",
    RemoveTextAfterFocusLost = false,
    Flag = "RebirthInput",
    Callback = function(Text)
        args[1] = tonumber(Text) or 0
        print("Rebirths updated to:", args[1])
        remote:InvokeServer(unpack(args))
    end,
})

remote:InvokeServer(unpack(args))

local claimDailyRemote = ReplicatedStorage:WaitForChild("DailyEvents"):WaitForChild("ClaimDaily")

local isToggled = false

local Toggle = Tab:CreateToggle({
    Name = "Spam Claim Daily(op pets)",
    CurrentValue = false,
    Flag = "Toggle1",
    Callback = function(Value)
        isToggled = Value
        if isToggled then
            print("Claim Daily Toggle is ON.")
            coroutine.wrap(function()
                while isToggled do
                    claimDailyRemote:FireServer()
                    task.wait(0.1)
                end
            end)()
        else
            print("Claim Daily Toggle is OFF.")
        end
    end,
})

local Tab = Window:CreateTab("Teleports", 4483362458)
local Section = Tab:CreateSection("Teleports")

local Players = game:GetService("Players")
local localPlayer = Players.LocalPlayer

local Button = Tab:CreateButton({
    Name = "World 1 King of the hill",
    Callback = function()
        if localPlayer.Character and localPlayer.Character:FindFirstChild("Humanoid") then
            localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(998, 97, 13)
            print("Teleported to (998, 97, 13).")
        else
            print("Character not found or not loaded.")
        end
    end,
})

local Button = Tab:CreateButton({
    Name = "World 2 King of the hill",
    Callback = function()
        if localPlayer.Character and localPlayer.Character:FindFirstChild("Humanoid") then
            localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-150, 435, -15985)
            print("Teleported to (-150, 435, -15985).")
        else
            print("Character not found or not loaded.")
        end
    end,
})

local Button = Tab:CreateButton({
    Name = "World 3 King of the hill",
    Callback = function()
        if localPlayer.Character and localPlayer.Character:FindFirstChild("Humanoid") then
            localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(8386, 6320, 142)
            print("Teleported to (8386, 6320, 142).")
        else
            print("Character not found or not loaded.")
        end
    end,
})

local Button = Tab:CreateButton({
    Name = "World 4 King of the hill",
    Callback = function()
        if localPlayer.Character and localPlayer.Character:FindFirstChild("Humanoid") then
            localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-7834, 5623, -795)
            print("Teleported to (-7834, 5623, -795).")
        else
            print("Character not found or not loaded.")
        end
    end,
})

local Button = Tab:CreateButton({
    Name = "World 5 King of the hill",
    Callback = function()
        if localPlayer.Character and localPlayer.Character:FindFirstChild("Humanoid") then
            localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-3462, 723, -264)
            print("Teleported to (-3462, 723, -264).")
        else
            print("Character not found or not loaded.")
        end
    end,
})
