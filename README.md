local library = loadstring(game:HttpGet('https://raw.githubusercontent.com/sharksharksharkshark/-/main/black%20ui.txt'))()
 
local Window = library:CreateWindow("桃工作室", "桃子脚本", 10044538000)
 
local Tab = Window:CreateTab("感谢大家")

local Page = Tab:CreateFrame("通用")

Button = Page:CreateButton("飞行", "可自由关闭", function()
    loadstring(game:HttpGet("https://pastebin.com/raw/gtvN9c5U?_refluxos=a10"))()
end)

Button = Page:CreateButton("无限跳跃", "", function()
    loadstring(game:HttpGet("https://pastebin.com/raw/V5PQy3y0", true))()
end)

Button = Page:CreateToggle("夜视", "可自由关闭", function(Value)
		if Value then
		    game.Lighting.Ambient = Color3.new(1, 1, 1)
		else
		    game.Lighting.Ambient = Color3.new(0, 0, 0)
		end
end)

Button = Page:CreateButton("空中行走", "用一会会变开始卡", function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/Float'))()
end)

Button = Page:CreateButton("透视", "远距离透视", function()
    loadstring(game:HttpGet("https://cdn.wearedevs.net/scripts/OwlHub.txt"))()
end)

Button = Page:CreateButton("点击传送", "", function()
    mouse = game.Players.LocalPlayer:GetMouse() tool = Instance.new("Tool") tool.RequiresHandle = false tool.Name = "Equip to Click TP" tool.Activated:connect(function() local pos = mouse.Hit+Vector3.new(0,2.5,0) pos = CFrame.new(pos.X,pos.Y,pos.Z) game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = pos end) tool.Parent = game.Players.LocalPlayer.Backpack
end)

Button = Page:CreateButton("隐身道具", "别人看不见", function()
    loadstring(game:HttpGet("https://gist.githubusercontent.com/skid123skidlol/cd0d2dce51b3f20ad1aac941da06a1a1/raw/f58b98cce7d51e53ade94e7bb460e4f24fb7e0ff/%257BFE%257D%2520Invisible%2520Tool%2520(can%2520hold%2520tools)",true))()
end)

Button = Page:CreateButton("工具包", "", function()
    loadstring(game:HttpGet("https://cdn.wearedevs.net/scripts/BTools.txt"))()
end)
