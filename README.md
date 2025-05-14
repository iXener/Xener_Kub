local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("Xener Kub Update 0.00000001 by iXener             Discord : Sigma ปะทะ 112💂‍♀️", "Ocean")
local Tab = Window:NewTab("1")
local Section = Tab:NewSection("เสกของ")
Section:NewButton("เสก", "ButtonInfo", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/yofriendfromschool1/Sky-Hub-Backup/main/gametoolgiver.lua"))()
end)
local Section = Tab:NewSection("Admin Panal")
Section:NewButton("Infyield", "ButtonInfo", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source"))()
end)
local Section = Tab:NewSection("Dex")
Section:NewButton("Infyiff", "ButtonInfo", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/infyiff/backup/main/dex.lua"))()
end)
local Section = Tab:NewSection("กด e/คลิก ไม่มี cooldown")
Section:NewButton("Hold no cooldown", "ButtonInfo", function()
    for e,e in pairs(game:GetService("Workspace"):GetDescendants()) do
	if e:IsA("ProximityPrompt") then
		e["HoldDuration"] = 0
	end
end
 
 
game:GetService("ProximityPromptService").PromptButtonHoldBegan:Connect(function(v)
    e["HoldDuration"] = 0
end)
end)
local Section = Tab:NewSection("บิน")
Section:NewButton("กด", "ButtonInfo", function()
    loadstring("\108\111\97\100\115\116\114\105\110\103\40\103\97\109\101\58\72\116\116\112\71\101\116\40\40\39\104\116\116\112\115\58\47\47\103\105\115\116\46\103\105\116\104\117\98\117\115\101\114\99\111\110\116\101\110\116\46\99\111\109\47\109\101\111\122\111\110\101\89\84\47\98\102\48\51\55\100\102\102\57\102\48\97\55\48\48\49\55\51\48\52\100\100\100\54\55\102\100\99\100\51\55\48\47\114\97\119\47\101\49\52\101\55\52\102\52\50\53\98\48\54\48\100\102\53\50\51\51\52\51\99\102\51\48\98\55\56\55\48\55\52\101\98\51\99\53\100\50\47\97\114\99\101\117\115\37\50\53\50\48\120\37\50\53\50\48\102\108\121\37\50\53\50\48\50\37\50\53\50\48\111\98\102\108\117\99\97\116\111\114\39\41\44\116\114\117\101\41\41\40\41\10\10")()
end)
local Section = Tab:NewSection("Fling (ใช้ได้เฉพาะแมพที่เดินชนกันแล้วไม่ทะลุ)")
Section:NewButton("Touch Fling Dino Anim", "ButtonInfo", function()
    loadstring(game:HttpGet(('https://raw.githubusercontent.com/0Ben1/fe/main/obf_K2n31uc6t2wY5A8786eR4K15sgbUF0vdQ80a0LzgvLRkSNYd89H1AS3124gMR6SM.lua.txt'),true))()
end)
Section:NewButton("Tounch Fling", "ButtonInfo", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/iXener/Fling/refs/heads/main/README.md"))()
end)
local Tab = Window:NewTab("2")
local Section = Tab:NewSection("2")
Section:NewButton("เปิดเสียงในแมพ(ไม่ได้ยิน = มีกันโปร)", "ButtonInfo", function()
    sound = true
local ID = "rbxassetid://4776398821" 
local Name = "get troll" 
local Volume = 100 
local Pitch = 100 

           for i,v in pairs(game:GetService("Workspace"):GetDescendants()) do
            if v:IsA("RemoteEvent") and v.Name == "AC6_FE_Sounds" then
                if sound == true then
                    v:FireServer("newSound", Name, workspace, ID, Pitch, Volume, true)
                    v:FireServer("playSound", Name)
                end 

                if sound == false then
                    v:FireServer("stopSound", Name)
                end
            end
        end
end)
Section:NewButton("ปิดเสียง)", "ButtonInfo", function()
    sound = false
local ID = "rbxassetid://4776398821" 
local Name = "get troll" 
local Volume = 100 
local Pitch = 100 

           for i,v in pairs(game:GetService("Workspace"):GetDescendants()) do
            if v:IsA("RemoteEvent") and v.Name == "AC6_FE_Sounds" then
                if sound == true then
                    v:FireServer("newSound", Name, workspace, ID, Pitch, Volume, true)
                    v:FireServer("playSound", Name)
                end 

                if sound == false then
                    v:FireServer("stopSound", Name)
                end
            end
        end
end)
Section:NewSlider("ปรับความเร็ววิ่ง", "SliderInfo", 500, 0, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)
Section:NewSlider("ปรับกระโดดสูง", "SliderInfo", 500, 0, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.JumpPower = s
end)
Section:NewButton("Aimbot", "ButtonInfo", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/thegod005/Mode/main/README.md"))()
end)
Section:NewButton("ชักว่าว(ใช้ได้เฉพาะแมพที่ใช้ R6)", "ButtonInfo", function()
    loadstring(game:HttpGet("https://pastefy.app/wa3v2Vgm/raw"))("Spider Script")
end)
Section:NewButton("GhostHub", "GhostHub(เมนูครบจบ)", function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/GhostHub'))()
end)
Section:NewButton("Anti AFK", "Anti AFK", function()
   local VirtualUser = game:GetService('VirtualUser')
 
game:GetService('Players').LocalPlayer.Idled:Connect(function()
    VirtualUser:CaptureController()
    VirtualUser:ClickButton2(Vector2.new())
end)
 
game:GetService("StarterGui"):SetCore("SendNotification", {
    Title = "AntiAFK loaded!",
    Text = "iXener",
    Button1 = "Have fun with Xener!!",
    Duration = 5
})
end)
Section:NewButton("วาปหาผู้เล่น", "Teleport players", function()
    loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/i1nZO9bkZb2Mljdy/raw",true))()
end)
local Tab = Window:NewTab("ตั้งปุ่ม เปิด/ปิด ui")
local Section = Tab:NewSection("เกี่ยวกับ UI")
Section:NewKeybind("กดหนึ่งที่แล้วเลือกปุ่มที่จะตั้ง", "KeybindInfo", Enum.KeyCode.F, function()
	Library:ToggleUI()
end)
