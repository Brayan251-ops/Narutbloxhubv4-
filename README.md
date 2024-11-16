--loadstring
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/Brayan251-ops/Wtf/refs/heads/main/source.lua"))()

--Windows
local Window = Library.CreateLib("Narutbloxscriptv4☠️", "BloodTheme")

--tabs
local Tab = Window:NewTab("v4")

--labels
Section:NewLabel("LabelText")


--comeco

--Button
Section:NewButton("🏠-MainFarm", "script blox fruits", function()
    print("Clicked")
end)


--toogles
Section:NewToggle("speed", "ToggleInfo", function(state)
    if state then
        print("speed On")
    else
        print("speed Off")
    end
end)

--sliders
Section:NewSlider("SliderText", "SliderInfo", 500, 0, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)
