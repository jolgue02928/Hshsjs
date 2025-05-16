-- Executa 20 vezes por segundo
while true do
    local args = {
        [1] = "Boat_5_Pad_5"
    }

    game:GetService("ReplicatedStorage").Network.Fishing_FishermanFish:InvokeServer(unpack(args))

    task.wait(0.05) -- 20 vezes por segundo
end
