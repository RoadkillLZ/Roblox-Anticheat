```Lua
# Roblox-Anticheat
A Roblox Anticheat that kicks a player when it detects speed and jump

local hum = script.Parent:WaitForChild("Humanoid")

while true do
  wait(1)
if hum.Walkspeed ~= 16 then
game.Players.LocalPlayer:Kick("The game has detected that you were speed hacking")
end
if hum.JumpPower ~= 50 then
game.Players.LocalPlayer:Kick("The game has detected that you were jump hacking")
end
end
