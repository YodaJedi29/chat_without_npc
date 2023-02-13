local Chat = game:GetService("Chat")

local npc = script.Parent
local characterParts = npc.CharacterParts
local head = characterParts.Head
local clickDetector = npc.ClickDetector

--Add table below
local dialogueArray= {"Oi tudo bem?" ,"De onde você vem", "Venho de Brumandinho","Vamos comer um Hamburguer?", "Sei um bom lugar" }

local function speak()

local dialogue = dialogueArray[1]
Chat:Chat(head, dialogue)
wait(1)
local dialogue = dialogueArray[2]
Chat:Chat(head, dialogue)
wait(1)
local dialogue = dialogueArray[3]
Chat:Chat(head, dialogue)
wait(1)
local dialogue = dialogueArray[4]
Chat:Chat(head, dialogue)
wait(1)
local dialogue = dialogueArray[5]
Chat:Chat(head, dialogue)
wait(1)
end

clickDetector.MouseClick:Connect(speak)
