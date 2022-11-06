local shadow=game:GetObjects("rbxassetid://1555932744")[1]
shadow.Parent = game.Players.LocalPlayer.Backpack
local anim = Instance.new("Animation")
anim.AnimationId = 'https://www.roblox.com/Assest?ID=9982615727'
local track
 
shadow.Equipped:Connect(function()
    track = game.Players.LocalPlayer.Character.Humanoid:LoadAnimation(anim) 
        track.Priority = Enum.AnimationPriority.Action
        track:Play()
        track.Looped = true
 
end)
 
shadow.Unequipped:Connect(function()
    if track then
        track:Stop()
    end
end)
