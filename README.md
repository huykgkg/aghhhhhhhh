local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("Bucu hub 2022", "Sentinel")

local Tab = Window:NewTab("Chicken")
local ScriptSection = Tab:NewSection("Arrow and Roka and idk")
ScriptSection:NewButton("Arrow", "Chikenezzez", function()
workspace.Pucci.Pucci:FireServer()
wait(1.5)
game:GetService("ReplicatedStorage").ItemEvent.StandArrow:FireServer()
end)

ScriptSection:NewButton("Roka just press arrow no need use this", "Chikenezzez", function()
workspace.Pucci.Pucci:FireServer()
end)

ScriptSection:NewButton("Weird Arrow", "Chikenezzez", function()
workspace.Pucci.Pucci:FireServer()
wait(1.5)
game:GetService("ReplicatedStorage").ItemEvent.WeirdArrow:FireServer()
end)

ScriptSection:NewButton("Shiny Mushroom", "Chikenezzez", function()
game:GetService("ReplicatedStorage").ItemEvent.ShinyMushroom:FireServer()
end)

local ScriptSection = Tab:NewSection("Get Quest")
ScriptSection:NewButton("Diego", "Chikenezzez", function()
local args = {
    [1] = "GetQuest",
    [2] = "JohnnyQuest"
}

game:GetService("ReplicatedStorage").prompt_service:FireServer(unpack(args))
end)

ScriptSection:NewButton("Dio", "Chikenezzez", function()
local args = {
    [1] = "GetQuest",
    [2] = "ZaiQuest"
}

game:GetService("ReplicatedStorage").prompt_service:FireServer(unpack(args))
end)

ScriptSection:NewButton("Soul Quest", "Chikenezzez", function()
local args = {
    [1] = "GetQuest",
    [2] = "HallowQuest"
}

game:GetService("ReplicatedStorage").prompt_service:FireServer(unpack(args))
end)

ScriptSection:NewButton("Kira", "Chikenezzez", function()
local args = {
    [1] = "GetQuest",
    [2] = "JosukeQuest"
}

game:GetService("ReplicatedStorage").prompt_service:FireServer(unpack(args))
end)

ScriptSection:NewButton("Diavolo", "Chikenezzez", function()
local args = {
    [1] = "GetQuest",
    [2] = "RisottoQuest"
}

game:GetService("ReplicatedStorage").prompt_service:FireServer(unpack(args))

end)

local ScriptSection = Tab:NewSection("Toggle gui")
ScriptSection:NewKeybind("Toggle Gui", "", Enum.KeyCode.RightControl, function()
	Library:ToggleUI()
end)
