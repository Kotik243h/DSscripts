getgenv().DanceHack = true  
local VirtualUser = game:GetService("VirtualUser")  
local VIM = game:GetService("VirtualInputManager")  

-- Активация по N + защита от античитов  
task.spawn(function()  
    while task.wait() do  
        if getgenv().DanceHack then  
            -- Имитация ручного ввода  
            VIM:SendKeyEvent(true, Enum.KeyCode.N, false, nil)  
            task.wait(0.1)  
            VIM:SendKeyEvent(false, Enum.KeyCode.N, false, nil)  

            -- Прямой триггер эмоции  
            game:GetService("Players").LocalPlayer.Character.Humanoid:PlayEmote("dance2")  

            -- Обход задержки эмоций  
            for i = 1, 3 do  
                VirtualUser:ClickButton2(Vector2.new())  
                task.wait(0.3)  
            end  
        end  
    end  
end)  

-- Выключить: execute("getgenv().DanceHack = false")  
