local TeleportService = game:GetService("TeleportService")
local servidorMoreira = "85d8bc8887a2de47909c44373bba59fb" -- ID do servidor

local function metodoMoreira()
    TeleportService:Teleport(servidorMoreira, game.Players.LocalPlayer)
end

-- criar um menu ou botão para chamar o método Moreira
local menu = Instance.new("ScreenGui")
local botao = Instance.new("TextButton")
botao.Text = "Método Moreira"
botao.Parent = menu
menu.Parent = game.Players.LocalPlayer.PlayerGui
botao.MouseButton1Click:Connect(metodoMoreira)
