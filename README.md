-- carregar biblioteca
local Fluent = loadstring(game:HttpGet("https://github.com/dawid-scripts/Fluent/releases/latest/download/main.lua"))()

-- janela principal

local Window = Fluent:CreateWindow({
    Title = "Cael Hub Brookhaven" .. Fluent.Version,
    TabWidth = 160, Size = UDim2.fromOffset(580, 460), Theme = "Dark"
})

-- abas

local Tabs = {
    Main = Window:AddTab({ Title = "Inicio" }),
    Settings = Window:AddTab({ Title = "Settings", Icon = "settings" })
}

-- notificacao

Fluent:Notify({ Title = "Notificação", Content = "Script iniciado com sucesso" })

-- parágrafo

Tabs.Main:AddParagraph({ Title = "Cael hub", Content = "Scripts de brookhaven" })
Tabs.Main:AddParagraph({ Title = "key do shadow", Content = "</>FaseTesting" })
Tabs.Main:AddParagraph({ Title = "key do dopamina", Content = "Graciasporseleccionarnos" })

-- botao

Tabs.Main:AddButton({ Title = "dopamina", Callback = function() script mega hubs:loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-Dopamina-Hub-17894"))() end })
Tabs.Main:AddButton({ Title = "shadow", Callback = function() Shadow:loadstring(game:HttpGet("https://raw.githubusercontent.com/xscripts7/XScripts/refs/heads/XScript/ShadowHub", true))() end })
Tabs.Main:AddButton({ Title = "sirius", Callback = function() loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-Sirius-7420"))() end })
Tabs.Main:AddButton({ Title = "sky", Callback = function() loadstring(game:HttpGet("https://raw.githubusercontent.com/yofriendfromschool1/Sky-Hub/main/SkyHub.txt"))() end })
Tabs.Main:AddButton({ Title = "sander x", Callback = function() Sander X 4 FLING Melhorando:loadstring(game:HttpGet('https://raw.githubusercontent.com/kigredns/SanderXV4.2.2/refs/heads/main/New.lua'))() end })
Tabs.Main:AddButton({ Title = "rael", Callback = function() loadstring(game:HttpGet"https://raw.githubusercontent.com/Laelmano24/Rael-Hub/main/main.txt")() end })

-- finalizar
Window:SelectTab(1)
Fluent:Notify({ Title = "Bem vindo", Content = "Script carregado com sucesso👍" })
