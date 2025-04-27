-- Script Lua para Bloqueio Azul no Roblox

local espAtivado = true
local fovAtivado = true
local setasAtivadas = true

local corEquipe = game.Players.LocalPlayer.TeamColor
local corInimigos = (corEquipe == BrickColor.new("Bright blue")) and BrickColor.new("Bright red") or BrickColor.new("Bright blue")

-- Função para alternar a ativação do script
function alternarScript()
    espAtivado = not espAtivado
    fovAtivado = not fovAtivado
    setasAtivadas = not setasAtivadas
end

-- Função para desenhar setas indicando a direção dos inimigos
function desenharSetas()
    -- Lógica para desenhar setas na tela apontando para os inimigos
end

-- Função para desenhar o FOV
function desenharFOV()
    -- Lógica para desenhar o círculo de FOV na tela
end

-- Função para desenhar o ESP
function desenharESP()
    -- Lógica para desenhar o ESP indicando a posição dos inimigos
end

-- Loop principal
while true do
    if espAtivado then
        desenharESP()
    end
    if fovAtivado then
        desenharFOV()
    end
    if setasAtivadas then
        desenharSetas()
    end
    wait(0.1) -- Atraso para evitar sobrecarga no processamento
end
