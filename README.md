local Remote = game:GetService("ReplicatedStorage"):WaitForChild("ChatSystemGetMessage") -- use dex check if got error

for i,v in pairs(game.Players:GetPlayers()) do
   if v.Character and v.Character:FindFirstChild("Humanoid") ~= nil and Remote then
       Remote:InvokeServer("hit", "}, {  ", math.huge, v.Character.Humanoid, "", 1.5)
   end
end
