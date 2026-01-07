# Cipher Library

## 📋 Introdução

**Compatibilidade:** Requer o ambiente `cipherBot` para inicialização.
**Dependências:** Módulos padrão do cliente OTClient (g_game, g_ui, g_map, etc.).
**Confiabilidade:** Esse arquivo foi gerado por uma IA, possivelmente terá bugs, porém a estrutura das funções estão iguais.

## 📑 Índice

### 🎨 UI Library
- [cipherBot.UI.create](#cipherbotuicreate)
- [cipherBot.UI.scrollbar](#cipherbotuiscrollbar)
- [cipherBot.UI.textedit](#cipherbotuitextedit)
- [cipherBot.UI.item](#cipherbotuiitem)
- [cipherBot.UI.switch](#cipherbotuiswitch)
- [cipherBot.UI.checkbox](#cipherbotuicheckbox)
- [cipherBot.UI.label](#cipherbotuilabel)
- [cipherBot.UI.separator](#cipherbotuiseparator)
- [cipherBot.UI.button](#cipherbotuibutton)
- [cipherBot.UI.combobox](#cipherbotuicombobox)
- [cipherBot.UI.section](#cipherbotuisection)
- [cipherBot.UI.clear](#cipherbotuiclear)
- [cipherBot.UI.icon](#cipherbotuiicon)
- [cipherBot.UI.scrollablePanel](#cipherbotuiscrollablepanel)
- [cipherBot.UI.clearStorage](#cipherbotuiclearstorage)
- [cipherBot.UI.clearStorageNamespace](#cipherbotuiclearstoragenamespace)

### 🧩 Widget Library
- [cipherBot.Widget.create](#cipherbotwidgetcreate)
- [cipherBot.Widget.changeText](#cipherbotwidgetchangetext)
- [cipherBot.Widget.changeVisibility](#cipherbotwidgetchangevisibility)
- [cipherBot.Widget.changeColor](#cipherbotwidgetchangecolor)
- [cipherBot.Widget.isVisible](#cipherbotwidgetisvisible)
- [cipherBot.Widget.changeImage](#cipherbotwidgetchangeimage)
- [cipherBot.Widget.changeSize](#cipherbotwidgetchangesize)
- [cipherBot.Widget.destroy](#cipherbotwidgetdestroy)
- [cipherBot.Widget.listWidgets](#cipherbotwidgetlistwidgets)

### 💾 Storage Library
- [cipherBot.getCurrentProfile](#cipherbotgetcurrentprofile)
- [cipherBot.profileCreate](#cipherbotprofilecreate)
- [cipherBot.profileSave](#cipherbotprofilesave)
- [cipherBot.profileOption](#cipherbotprofileoption)
- [cipherBot.profileJson](#cipherbotprofilejson)
- [cipherBot.newProfile](#cipherbotnewprofile)
- [cipherBot.getProfilesName](#cipherbotgetprofilesname)
- [cipherBot.changeProfile](#cipherbotchangeprofile)
- [cipherBot.onProfileChange](#cipherbotonprofilechange)
- [cipherBot.doLoadFile](#cipherbotdoloadfile)
- [cipherBot.doSaveFile](#cipherbotdosavefile)
- [cipherBot.doWorldSave](#cipherbotdoworldsave)
- [cipherBot.doWorldLoading](#cipherbotdoworldloading)

### ⚙️ Core Library
- [cipherBot.getSpectators](#cipherbotgetspectators)
- [cipherBot.getCreatureByName](#cipherbotgetcreaturebyname)
- [cipherBot.getCreatureById](#cipherbotgetcreaturebyid)
- [cipherBot.doAttack](#cipherbotdoattack)
- [getCreature](#getcreature)
- [getTarget](#gettarget)
- [getCreatureByType](#getcreaturebytype)
- [getCreatureByEmblem](#getcreaturebyemblem)
- [getCreatureBySkull](#getcreaturebyskull)
- [distanceFromPlayer](#distancefromplayer)
- [isFacingTarget](#isfacingtarget)
- [samePos](#samepos)
- [comparePzPositions](#comparepzpositions)
- [cipherBot.tr](#cipherbottr)
- [isDragKeyPressed](#isdragkeypressed)
- [cipherBot.isKeyPressed](#cipherbotiskeypressed)
- [doTempLoadFile](#dotemploadfile)
- [swapTableElements](#swaptableelements)
- [showSkillLevel](#showskilllevel)
- [calcStamina](#calcstamina)
- [itemAmount](#itemamount)
- [getFirstNumberInText](#getfirstnumberintext)
- [isValidSize](#isvalidsize)
- [extractSpecificTextInString](#extractspecifictextinstring)
- [firstLetterUpper](#firstletterupper)
- [compareLowerStrings](#comparelowerstrings)
- [generateRandomString](#generaterandomstring)
- [doFormatTime](#doformattime)
- [automaticPercentage](#automaticpercentage)
- [doDownloadImage](#dodownloadimage)
- [doCast](#docast)
- [getAttackerName](#getattackername)
- [getAttackersCount](#getattackerscount)
- [getTabs](#gettabs)
- [cipherBot.getMacroStorage](#cipherbotgetmacrostorage)
- [cipherBot.createMacroSettings](#cipherbotcreatemacrosettings)
- [cipherBot.getMacroName](#cipherbotgetmacroname)
- [cipherBot.getMacroKey](#cipherbotgetmacrokey)
- [cipherBot.getMacroDelay](#cipherbotgetmacrodelay)
- [cipherBot.getMacroTab](#cipherbotgetmacrotab)
- [cipherBot.getMacroIcon](#cipherbotgetmacroicon)
- [cipherBot.isScriptEnabled](#cipherbotisscriptenabled)
- [cipherBot.registerMacroSettings](#cipherbotregistermacrosettings)
- [cipherBot.setMacroName](#cipherbotsetmacroname)
- [cipherBot.setMacroKey](#cipherbotsetmacrokey)
- [cipherBot.setMacroDelay](#cipherbotsetmacrodelay)
- [cipherBot.setMacroTab](#cipherbotsetmacrotab)
- [cipherBot.setMacroIcon](#cipherbotsetmacroicon)
- [cipherBot.deleteMacro](#cipherbotdeletemacro)
- [cipherBot.listMacros](#cipherbotlistmacros)
- [cipherBot.resetMacro](#cipherbotresetmacro)
- [cipherBot.cloneMacro](#cipherbotclonemacro)
- [cipherBot.macroExists](#cipherbotmacroexists)
- [cipherBot.updateMacro](#cipherbotupdatemacro)
- [cipherBot.macro](#cipherbotmacro)
- [cipherBot.setDefaultTab](#cipherbotsetdefaulttab)
- [cipherBot.getCurrentTab](#cipherbotgetcurrenttab)
- [cipherBot.listTabs](#cipherbotlisttabs)
- [cipherBot.tabExists](#cipherbottabexists)
- [insertSpellList](#insertspelllist)

### 🎯 Icon Library
- [cipherBot.Icon.create](#cipherboticoncreate)
- [cipherBot.Icon.changeVisibility](#cipherboticonchangevisibility)
- [cipherBot.Icon.setCallback](#cipherboticonsetcallback)
- [cipherBot.Icon.setText](#cipherboticonsettext)
- [cipherBot.Icon.setColor](#cipherboticonsetcolor)
- [cipherBot.Icon.setItem](#cipherboticonsetitem)
- [cipherBot.Icon.setOutfit](#cipherboticonsetoutfit)
- [cipherBot.Icon.setOn](#cipherboticonseton)
- [cipherBot.Icon.setOff](#cipherboticonsetoff)
- [cipherBot.Icon.isOn](#cipherboticonison)
- [cipherBot.Icon.remove](#cipherboticonremove)

### 🔔 Alert Library
- [cipherBot.showAlert](#cipherbotshowalert)

---

## ⚡ Quick Start
```lua
-- Exemplo básico de uso
if (not cipherBot) then return end

-- Criar uma janela principal
local window = cipherBot.UI.create("Minha Janela", 400, 300)

-- Adicionar um botão
cipherBot.UI.button("Clique aqui", function()
    cipherBot.showAlert({
        title = "Sucesso",
        message = "Botão clicado!",
        duration = 2000
    })
end, window.mainPanel)

-- Criar um widget personalizado
cipherBot.Widget.create("meuWidget", "Status", "#00FF00")
```

---

## 🎨 UI Library

### cipherBot.UI.create

Cria uma janela principal redimensionável e arrastável com gerenciamento automático de posição.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| text | string | Sim | "Mrl Scripts" | Título da janela |
| width | number | Sim | 300 | Largura em pixels |
| height | number | Sim | 250 | Altura em pixels |
| windowId | string | Sim | valor de text | Identificador único da janela |
| isSimple | boolean | Sim | false | Se true, cria SimpleCipherWindow |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Widget da janela criada |
| string | Mensagem de erro em caso de falha |

#### Exemplo
```lua
-- Criar janela padrão
local window = cipherBot.UI.create("Configurações", 400, 300)

-- Criar janela simples
local simpleWindow = cipherBot.UI.create("Simples", 200, 150, "minhaJanela", true)
```

#### Notas
- A posição da janela é automaticamente centralizada
- Janelas anteriores com mesmo ID são destruídas
- Suporte para temas simples (SimpleCipherWindow) e completos (CipherWindow)

---

### cipherBot.UI.scrollbar

Cria uma barra de rolagem horizontal com persistência de valor.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| storageName | string | Não | — | Namespace de armazenamento |
| id | string | Não | — | Identificador único no namespace |
| title | string | Não | — | Rótulo exibido acima da barra |
| min | number | Não | — | Valor mínimo |
| max | number | Não | — | Valor máximo |
| defaultValue | number | Não | — | Valor inicial/padrão |
| dest | table | Não | — | Widget pai para anexar |
| tooltip | string | Sim | nil | Texto de tooltip |
| options | table | Sim | {} | Opções adicionais |

#### Opções
| Opção | Tipo | Padrão | Descrição |
| :--- | :--- | :--- | :--- |
| enableStorage | boolean | true | Ativar persistência do valor |
| onChange | function | nil | Callback quando valor muda |
| clearOnDestroy | boolean | false | Limpar storage ao destruir widget |
| format | string | "none" | Modo: "none", "percent", "time" |
| timeMode | string | "auto" | Modo de tempo: "s", "m:s", "h:m:s", "d:h:m:s", "auto" |
| timeInMillis | boolean | false | Se o tempo está em milissegundos |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Widget da barra de rolagem |

#### Exemplo
```lua
-- Barra de rolagem simples
local scroll = cipherBot.UI.scrollbar("config", "volume", "Volume", 0, 100, 50, parent)

-- Barra de rolagem com formato percentual
local percentScroll = cipherBot.UI.scrollbar("ui", "opacity", "Opacidade", 0, 100, 80, parent, nil, {
    format = "percent",
    onChange = function(value)
        print("Opacidade alterada para: " .. value)
    end
})
```

#### Performance
- Tempo de execução: ~3ms
- Atualizações suaves com callback otimizado

---

### cipherBot.UI.textedit

Cria um campo de entrada de texto com persistência automática.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| storageName | string | Não | — | Namespace de armazenamento |
| id | string | Não | — | Identificador único |
| title | string | Não | — | Rótulo acima do campo |
| defaultValue | string | Não | — | Valor inicial |
| dest | table | Não | — | Widget pai |
| tooltip | string | Sim | nil | Texto de tooltip |
| options | table | Sim | {} | Opções adicionais |

#### Opções
| Opção | Tipo | Padrão | Descrição |
| :--- | :--- | :--- | :--- |
| enableStorage | boolean | true | Persistir texto |
| onChange | function | nil | Callback ao alterar texto |
| clearOnDestroy | boolean | false | Limpar storage ao destruir |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Widget do campo de texto |

#### Exemplo
```lua
-- Campo de texto simples
local nameField = cipherBot.UI.textedit("player", "name", "Nome do Personagem", "", parent)

-- Campo com validação
local emailField = cipherBot.UI.textedit("config", "email", "E-mail", "user@example.com", parent, nil, {
    onChange = function(text)
        if not text:match("%S+@%S+%.%S+") then
            cipherBot.showAlert({title = "Erro", message = "E-mail inválido"})
        end
    end
})
```

---

### cipherBot.UI.item

Cria um seletor de itens com persistência de ID.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| storageName | string | Não | — | Namespace de armazenamento |
| id | string | Não | — | Identificador único |
| title | string | Não | — | Rótulo ao lado do seletor |
| defaultItem | number/string | Não | — | ID do item padrão |
| dest | table | Não | — | Widget pai |
| tooltip | string | Sim | nil | Texto de tooltip |
| options | table | Sim | {} | Opções adicionais |

#### Opções
| Opção | Tipo | Padrão | Descrição |
| :--- | :--- | :--- | :--- |
| enableStorage | boolean | true | Persistir ID do item |
| onChange | function | nil | Callback ao alterar item |
| clearOnDestroy | boolean | false | Limpar storage ao destruir |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Widget do seletor de itens |

#### Exemplo
```lua
-- Seletor de item básico
local potionSelector = cipherBot.UI.item("config", "healingPotion", "Poção de Cura", 7618, parent)

-- Seletor com callback
local weaponSelector = cipherBot.UI.item("equipment", "weapon", "Arma", 2376, parent, nil, {
    onChange = function(itemId)
        print("Arma selecionada: " .. itemId)
    end
})
```

---

### cipherBot.UI.switch

Cria um interruptor de alternância com persistência de estado.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| storageName | string | Não | — | Namespace de armazenamento |
| id | string | Não | — | Identificador único |
| title | string | Não | — | Texto do interruptor |
| defaultValue | boolean | Não | — | Estado inicial (on/off) |
| dest | table | Não | — | Widget pai |
| tooltip | string | Sim | nil | Texto de tooltip |
| options | table | Sim | {} | Opções adicionais |

#### Opções
| Opção | Tipo | Padrão | Descrição |
| :--- | :--- | :--- | :--- |
| enableStorage | boolean | true | Persistir estado |
| onChange | function | nil | Callback ao alternar |
| clearOnDestroy | boolean | false | Limpar storage ao destruir |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Widget do interruptor |

#### Exemplo
```lua
-- Interruptor simples
local toggle = cipherBot.UI.switch("config", "autoHeal", "Auto Heal", false, parent)

-- Interruptor com ação
local autoAttack = cipherBot.UI.switch("combat", "autoAttack", "Auto Ataque", true, parent, "Ativar ataque automático", {
    onChange = function(isOn)
        if isOn then
            schedule(100, function() attackNearest() end)
        end
    end
})
```

---

### cipherBot.UI.checkbox

Cria uma caixa de seleção com estado persistente.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| storageName | string | Não | — | Namespace de armazenamento |
| id | string | Não | — | Identificador único |
| title | string | Não | — | Texto ao lado da caixa |
| defaultValue | boolean | Não | — | Estado inicial |
| dest | table | Não | — | Widget pai |
| tooltip | string | Sim | nil | Texto de tooltip |
| callback | function | Sim | nil | Callback legado |
| options | table | Sim | {} | Opções adicionais |

#### Opções
| Opção | Tipo | Padrão | Descrição |
| :--- | :--- | :--- | :--- |
| enableStorage | boolean | true | Persistir estado |
| onChange | function | nil | Callback ao alterar |
| clearOnDestroy | boolean | false | Limpar storage ao destruir |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Widget da caixa de seleção |

#### Exemplo
```lua
-- Checkbox básico
local option = cipherBot.UI.checkbox("config", "showNames", "Mostrar Nomes", true, parent)

-- Checkbox com múltiplas ações
local notifications = cipherBot.UI.checkbox("ui", "notifications", "Notificações", true, parent, nil, function(checked)
    if checked then
        enableNotifications()
    else
        disableNotifications()
    end
end, {
    clearOnDestroy = true
})
```

---

### cipherBot.UI.label

Cria um rótulo de texto simples.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| text | string | Não | — | Conteúdo do texto |
| dest | table | Não | — | Widget pai |
| labelType | string | Sim | "CipherTextLabel" | Classe de estilo |
| tooltip | string | Sim | nil | Texto de tooltip |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Widget do rótulo |

#### Exemplo
```lua
-- Rótulo simples
cipherBot.UI.label("Status: Online", parent)

-- Rótulo com estilo personalizado
cipherBot.UI.label("Aviso Importante", parent, "CipherTitleLabel", "Clique para detalhes")
```

---

### cipherBot.UI.separator

Cria uma linha separadora horizontal para organização visual.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| dest | table | Não | — | Widget pai |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Widget do separador |

#### Exemplo
```lua
-- Separador entre seções
cipherBot.UI.separator(parent)
```

---

### cipherBot.UI.button

Cria um botão clicável.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| text | string | Não | — | Texto do botão |
| callback | function | Sim | nil | Função executada ao clicar |
| parent | table | Não | — | Widget pai |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Widget do botão |

#### Exemplo
```lua
-- Botão com ação
cipherBot.UI.button("Salvar", function(btn)
    saveConfig()
    btn:setText("Salvo!")
end, parent)

-- Botão sem callback (para uso posterior)
local myButton = cipherBot.UI.button("Clique-me", nil, parent)
myButton.onClick = function()
    print("Botão clicado!")
end
```

---

### cipherBot.UI.combobox

Cria uma lista suspensa com seleção persistente.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| storageName | string | Não | — | Namespace de armazenamento |
| id | string | Não | — | Identificador único |
| text | string | Não | — | Texto do rótulo |
| options | table | Não | — | Lista de opções |
| defaultValue | string | Não | — | Opção inicial |
| dest | table | Não | — | Widget pai |
| tooltip | string | Sim | nil | Texto de tooltip |
| callback | function | Sim | nil | Callback legado |
| extraOptions | table | Sim | {} | Opções adicionais |

#### Opções
| Opção | Tipo | Padrão | Descrição |
| :--- | :--- | :--- | :--- |
| enableStorage | boolean | true | Persistir seleção |
| onChange | function | nil | Callback ao alterar |
| clearOnDestroy | boolean | false | Limpar storage ao destruir |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Widget do combobox |

#### Exemplo
```lua
-- Combobox simples
local classSelector = cipherBot.UI.combobox("player", "class", "Classe", 
    {"Guerreiro", "Mago", "Arqueiro"}, "Guerreiro", parent)

-- Combobox dinâmico
local serverSelector = cipherBot.UI.combobox("config", "server", "Servidor", 
    getServerList(), "Antica", parent, nil, nil, {
        onChange = function(selected)
            connectToServer(selected)
        end
    })
```

---

### cipherBot.UI.section

Cria um painel de seção com título opcional para agrupar widgets.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| titleText | string | Sim | nil | Texto do título |
| dest | table | Não | — | Widget pai |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Widget da seção |

#### Exemplo
```lua
-- Seção com título
local combatSection = cipherBot.UI.section("Configurações de Combate", parent)

-- Seção sem título (apenas container)
local container = cipherBot.UI.section(nil, parent)
```

---

### cipherBot.UI.clear

Remove todos os widgets filhos de um widget pai.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| widget | table | Não | — | Widget pai |

#### Exemplo
```lua
-- Limpar painel
cipherBot.UI.clear(myPanel)
```

---

### cipherBot.UI.icon

Cria um widget de ícone/imagem.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| imagePath | string | Não | — | Caminho da imagem |
| dest | table | Não | — | Widget pai |
| tooltip | string | Sim | nil | Texto de tooltip |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Widget do ícone |

#### Exemplo
```lua
-- Ícone de arquivo local
cipherBot.UI.icon("/images/icon.png", parent, "Ícone de alerta")

-- Ícone de URL (se suportado)
cipherBot.UI.icon("https://example.com/icon.png", parent)
```

---

### cipherBot.UI.scrollablePanel

Cria um painel rolável com barra de rolagem vertical.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | Descrição |
| title | string | Sim | — | Título (não utilizado na implementação) |
| parent | table | Não | — | Widget pai |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Tabela com `window` (painel) e `list` (container de conteúdo) |

#### Exemplo
```lua
-- Criar painel rolável
local scrollPanel = cipherBot.UI.scrollablePanel("Itens", mainWindow)

-- Adicionar itens à lista
for i = 1, 50 do
    cipherBot.UI.label("Item " .. i, scrollPanel.list)
end
```

---

### cipherBot.UI.clearStorage

Remove uma chave específica de um namespace de armazenamento.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| storageName | string | Não | — | Namespace de armazenamento |
| key | string | Não | — | Chave específica para remover |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se limpo, false se não encontrado |

#### Exemplo
```lua
-- Limpar configuração específica
local success = cipherBot.UI.clearStorage("config", "volume")
if success then
    print("Volume resetado")
end
```

---

### cipherBot.UI.clearStorageNamespace

Remove completamente um namespace de armazenamento e todas as suas chaves.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| storageName | string | Não | — | Namespace para remover |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se limpo, false se não encontrado |

#### Exemplo
```lua
-- Limpar todas as configurações de UI
cipherBot.UI.clearStorageNamespace("uiSettings")
```

---

## 🧩 Widget Library

### cipherBot.Widget.create

Cria um widget personalizado arrastável com persistência de posição e aparência.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| widgetName | string | Não | — | Identificador único do widget |
| title | string | Não | — | Título inicial do widget |
| color | string | Sim | — | Cor inicial (formato HEX) |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Widget criado ou nil |

#### Exemplo
```lua
-- Criar widget de status
local statusWidget = cipherBot.Widget.create("playerStatus", "HP: 100%", "#00FF00")

-- Widget com cor personalizada
local expWidget = cipherBot.Widget.create("expTracker", "EXP: 0%", "#9D4EDD")
```

#### Notas
- Widgets são automaticamente salvos no storage
- Suporta arrastar com tecla Ctrl (desktop) ou F2 (mobile)
- Posição é persistida entre sessões

---

### cipherBot.Widget.changeText

Altera o texto de um widget existente.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| widgetName | string | Não | — | Identificador do widget |
| newText | string | Não | — | Novo texto |
| saveText | boolean | Sim | true | Salvar texto no storage |

#### Exemplo
```lua
-- Atualizar texto do widget
cipherBot.Widget.changeText("playerStatus", "HP: 85%")

-- Atualizar sem salvar (temporário)
cipherBot.Widget.changeText("expTracker", "EXP: 45%", false)
```

---

### cipherBot.Widget.changeVisibility

Altera a visibilidade de um widget.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| widgetName | string | Não | — | Identificador do widget |
| visible | boolean | Não | — | true para mostrar, false para esconder |

#### Exemplo
```lua
-- Esconder widget
cipherBot.Widget.changeVisibility("playerStatus", false)

-- Mostrar widget
cipherBot.Widget.changeVisibility("expTracker", true)
```

---

### cipherBot.Widget.changeColor

Altera a cor do texto de um widget.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| widgetName | string | Não | — | Identificador do widget |
| color | string | Não | — | Nova cor (formato HEX) |

#### Exemplo
```lua
-- Mudar cor para vermelho (baixa saúde)
cipherBot.Widget.changeColor("playerStatus", "#FF0000")

-- Mudar cor para amarelo (alerta)
cipherBot.Widget.changeColor("expTracker", "#FFFF00")
```

---

### cipherBot.Widget.isVisible

Verifica se um widget está visível.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| widgetName | string | Não | — | Identificador do widget |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se visível, false caso contrário |

#### Exemplo
```lua
-- Verificar visibilidade
if cipherBot.Widget.isVisible("playerStatus") then
    print("Widget de status está visível")
end
```

---

### cipherBot.Widget.changeImage

Altera a imagem de um widget (requer função doDownloadImage).

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| widgetName | string | Não | — | Identificador do widget |
| url | string | Não | — | URL da imagem |
| type | string | Não | — | Tipo de imagem: "icon" ou "image" |

#### Exemplo
```lua
-- Alterar ícone do widget
cipherBot.Widget.changeImage("playerStatus", "https://example.com/icon.png", "icon")

-- Alterar imagem de fundo
cipherBot.Widget.changeImage("expTracker", "/images/background.png", "image")
```

#### Notas
- Requer a função `doDownloadImage` disponível globalmente
- Suporta URLs remotas e arquivos locais

---

### cipherBot.Widget.changeSize

Altera o tamanho de um widget.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| widgetName | string | Não | — | Identificador do widget |
| size | table | Não | — | Tabela com campos x (largura) e y (altura) |

#### Exemplo
```lua
-- Aumentar tamanho do widget
cipherBot.Widget.changeSize("playerStatus", {x = 150, y = 40})

-- Reduzir tamanho do widget
cipherBot.Widget.changeSize("expTracker", {x = 100, y = 30})
```

---

### cipherBot.Widget.destroy

Destroi um widget e o remove do storage.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| widgetName | string | Não | — | Identificador do widget |

#### Exemplo
```lua
-- Remover widget
cipherBot.Widget.destroy("playerStatus")
```

---

### cipherBot.Widget.listWidgets

Lista todos os widgets ativos.

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Nomes de todos os widgets ativos |

#### Exemplo
```lua
-- Listar widgets
local widgets = cipherBot.Widget.listWidgets()
for _, name in ipairs(widgets) do
    print("Widget: " .. name)
end
```

---

## 💾 Storage Library

### cipherBot.getCurrentProfile

Obtém o perfil atual do jogador.

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| string | Nome do perfil atual |

#### Exemplo
```lua
local currentProfile = cipherBot.getCurrentProfile()
print("Perfil atual: " .. currentProfile)
```

---

### cipherBot.profileCreate

Cria um perfil padrão para o jogador atual se não existir.

#### Exemplo
```lua
-- Criar perfil inicial
cipherBot.profileCreate()
```

#### Notas
- Cria perfil com nome do jogador como padrão
- Inicializa arquivos JSON necessários

---

### cipherBot.profileSave

Salva os dados do perfil atual no arquivo.

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se salvo com sucesso |

#### Exemplo
```lua
-- Forçar salvamento
local success = cipherBot.profileSave()
if success then
    print("Perfil salvo com sucesso")
end
```

---

### cipherBot.profileOption

Carrega e exibe as opções de perfil disponíveis no combobox.

#### Exemplo
```lua
-- Atualizar lista de perfis
cipherBot.profileOption()
```

---

### cipherBot.profileJson

Cria ou verifica o arquivo JSON para um perfil específico.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| profileName | string | Não | — | Nome do perfil |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se arquivo existe/criado |

#### Exemplo
```lua
-- Criar arquivo para perfil
cipherBot.profileJson("MeuPerfil")
```

---

### cipherBot.newProfile

Cria um novo perfil com storage vazio.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| profileName | string | Não | — | Nome do novo perfil |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se criado com sucesso |

#### Exemplo
```lua
-- Criar novo perfil
local success = cipherBot.newProfile("Hardcore")
if success then
    print("Perfil criado")
end
```

---

### cipherBot.getProfilesName

Obtém lista de nomes de todos os perfis disponíveis.

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Array com nomes dos perfis |

#### Exemplo
```lua
-- Listar perfis
local profiles = cipherBot.getProfilesName()
for _, name in ipairs(profiles) do
    print("Perfil: " .. name)
end
```

---

### cipherBot.changeProfile

Altera o perfil atual do jogador.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| profileName | string | Não | — | Nome do perfil para mudar |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se alterado com sucesso |

#### Exemplo
```lua
-- Mudar perfil
local changed = cipherBot.changeProfile("Hardcore")
if changed then
    print("Perfil alterado")
end
```

---

### cipherBot.onProfileChange

Callback chamado quando o perfil é alterado (pode ser sobrescrito).

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| oldProfile | string | Não | — | Perfil anterior |
| newProfile | string | Não | — | Novo perfil |

#### Exemplo
```lua
-- Sobrescrever comportamento
cipherBot.onProfileChange = function(oldProfile, newProfile)
    print("Perfil alterado de " .. oldProfile .. " para " .. newProfile)
    -- Carregar configurações específicas do perfil
end
```

---

### cipherBot.doLoadFile

Carrega dados do arquivo JSON do perfil atual.

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se carregado com sucesso |

#### Exemplo
```lua
-- Carregar dados do perfil
cipherBot.doLoadFile()
```

#### Notas
- Inicializa `cipherBot.storage` com dados do perfil
- Cria estrutura padrão se arquivo não existe

---

### cipherBot.doSaveFile

Salva dados do perfil atual no arquivo JSON.

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se salvo com sucesso |

#### Exemplo
```lua
-- Salvar dados do perfil
local saved = cipherBot.doSaveFile()
```

---

### cipherBot.doWorldSave

Salva dados específicos do mundo atual.

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se salvo com sucesso |

#### Exemplo
```lua
-- Salvar dados do mundo
cipherBot.doWorldSave()
```

---

### cipherBot.doWorldLoading

Carrega dados específicos do mundo atual.

#### Exemplo
```lua
-- Carregar dados do mundo
cipherBot.doWorldLoading()
```

---

## ⚙️ Core Library

### cipherBot.getSpectators

Obtém todos os espectadores (criaturas) no andar atual.

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Todas as criaturas no andar atual |

#### Exemplo
```lua
local spectators = cipherBot.getSpectators()
print(#spectators .. " criaturas no andar")
```

---

### cipherBot.getCreatureByName

Procura uma criatura pelo nome.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| name | string | Não | — | Nome da criatura |
| multifloor | boolean | Sim | false | Buscar em múltiplos andares |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Criatura encontrada ou nil |

#### Exemplo
```lua
local target = cipherBot.getCreatureByName("Dragon Lord")
if target then
    cipherBot.doAttack(target)
end
```

---

### cipherBot.getCreatureById

Procura uma criatura pelo ID.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| id | number | Não | — | ID da criatura |
| multifloor | boolean | Sim | false | Buscar em múltiplos andares |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Criatura encontrada ou nil |

#### Exemplo
```lua
local creature = cipherBot.getCreatureById(12345)
if creature then
    print("Criatura encontrada: " .. creature:getName())
end
```

---

### cipherBot.doAttack

Executa ataque a uma criatura alvo.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| target | table | Não | — | Criatura alvo |

#### Exemplo
```lua
local target = cipherBot.getCreatureByName("Dragon Lord")
if target then
    cipherBot.doAttack(target)
end
```

#### Notas
- Verifica se pode realizar ação de jogo
- Cancela follow se estiver seguindo o alvo
- Gerencia protocolo de ataque adequadamente

---

### getCreature

Busca criaturas dentro de uma área especificada com vários filtros.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| data | table | Não | — | Parâmetros de busca |

#### Estrutura de `data`
| Campo | Tipo | Padrão | Descrição |
| :--- | :--- | :--- | :--- |
| creature | string | "creature" | Tipo: 'creature', 'player', 'npc', 'monster' |
| area | number | 10 | Raio de busca |
| multifloor | boolean | false | Incluir múltiplos andares |
| byId | boolean | false | Filtrar por ID |
| id | number | nil | ID específico |
| byName | boolean | false | Filtrar por nome |
| name | string | nil | Nome específico |
| health | number | false | Percentual máximo de vida |
| attackers | boolean | false | Apenas atacantes |
| byEmblem | boolean | false | Filtrar por emblema |
| emblem | number/table | nil | Emblema(s) específico(s) |
| byShield | boolean | false | Filtrar por skull |
| shield | number/table | nil | Skull(s) específico(s) |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| number | Contagem total de criaturas |
| boolean | true se pelo menos uma encontrada |
| table | Detalhes das criaturas encontradas |

#### Exemplo
```lua
-- Buscar players atacantes com menos de 50% de vida
local count, found, details = getCreature({
    creature = "player",
    area = 7,
    health = 50,
    attackers = true
})

if found then
    print(count .. " players atacando com baixa vida")
end
```

---

### getTarget

Busca informações sobre o alvo atual com filtros.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| data | table | Não | — | Parâmetros de busca |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| number | 1 se alvo corresponde aos filtros, 0 caso contrário |
| boolean | true se alvo corresponde |
| table | Detalhes do alvo |

#### Exemplo
```lua
-- Verificar se alvo é um monstro com menos de 30% de vida
local count, isMonsterLowHP = getTarget({
    creature = "monster",
    health = 30
})

if isMonsterLowHP then
    print("Alvo é monstro com vida baixa")
end
```

---

### getCreatureByType

Verifica o tipo de uma criatura.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| creatureType | string | Não | — | Tipo: 'player', 'creature', 'npc', 'monster' |
| spec | table | Não | — | Especificação da criatura |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se a criatura corresponde ao tipo |

#### Exemplo
```lua
local isPlayer = getCreatureByType("player", creature)
```

---

### getCreatureByEmblem

Verifica se uma criatura possui emblema específico.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| emblemType | number/table | Não | — | Emblema(s) para verificar |
| spec | table | Não | — | Especificação da criatura |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se a criatura tem o emblema |

#### Exemplo
```lua
-- Verificar se é inimigo (emblema 2 ou 3)
local isEnemy = getCreatureByEmblem({2, 3}, creature)
```

---

### getCreatureBySkull

Verifica se uma criatura possui skull específico.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| skullType | number/table | Não | — | Skull(s) para verificar |
| spec | table | Não | — | Especificação da criatura |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se a criatura tem o skull |

#### Exemplo
```lua
-- Verificar skull vermelho (4)
local isRedSkull = getCreatureBySkull(4, creature)
```

---

### distanceFromPlayer

Calcula a distância do jogador até coordenadas especificadas.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| coords | table | Não | — | Coordenadas {x, y, z} |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| number | Distância até as coordenadas |

#### Exemplo
```lua
local dist = distanceFromPlayer({x = 100, y = 100, z = 7})
print("Distância: " .. dist)
```

---

### isFacingTarget

Verifica se o jogador está virado para o alvo dentro de uma distância.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| player | table | Não | — | Criatura jogador |
| target | table | Não | — | Criatura alvo |
| distance | number | Sim | 8 | Distância máxima |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se está virado para o alvo |

#### Exemplo
```lua
local facing = isFacingTarget(player, target, 5)
if facing then
    say("exori")
end
```

---

### samePos

Compara se duas posições são iguais.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| pos1 | table | Não | — | Primeira posição {x, y, z} |
| pos2 | table | Não | — | Segunda posição {x, y, z} |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se posições são iguais |

#### Exemplo
```lua
local playerPos = pos()
local targetPos = target():getPosition()
if samePos(playerPos, targetPos) then
    print("Na mesma posição")
end
```

---

### comparePzPositions

Verifica e adiciona posição de PZ (Protected Zone) à lista.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| position | table | Não | — | Posição para verificar |
| tab | table | Não | — | Tabela de posições |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se posição foi adicionada |

#### Exemplo
```lua
local wasAdded = comparePzPositions(player:getPosition(), cipherBot.storageWorld.pzTiles)
if wasAdded then
    print("Nova posição PZ adicionada")
end
```

---

### cipherBot.tr

Função de tradução para mensagens da biblioteca.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| message | string | Não | — | Mensagem para traduzir |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| string | Mensagem traduzida ou original |

#### Exemplo
```lua
local translated = cipherBot.tr("Profile Error")
```

#### Notas
- Usa configuração de idioma do storage
- Fallback para português brasileiro
- Suporta pt_br, en_us, pl_pl

---

### isDragKeyPressed

Verifica se a tecla de arrastar está pressionada.

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se tecla pressionada |

#### Notas
- Mobile: Botão F2
- Desktop: Tecla Ctrl

---

### cipherBot.isKeyPressed

Verifica se uma tecla ou botão do mouse está pressionado.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| input | string | Não | — | Tecla ou "Mouse1"-"Mouse9" |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se pressionado |

#### Exemplo
```lua
if cipherBot.isKeyPressed("Ctrl+Space") then
    print("Atalho pressionado")
end

if cipherBot.isKeyPressed("Mouse1") then
    print("Botão esquerdo pressionado")
end
```

---

### doTempLoadFile

Carrega temporariamente dados de um arquivo JSON.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| path | string | Não | — | Caminho do arquivo |
| table | table | Não | — | Tabela para armazenar dados |
| searchKey | string | Não | — | Chave para buscar |
| save | boolean | Sim | false | Salvar após carregar |

#### Exemplo
```lua
-- Carregar configurações temporárias
doTempLoadFile("/bot/config.json", tempSettings, "keybinds")
```

---

### swapTableElements

Troca dois elementos em uma tabela.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| tbl | table | Não | — | Tabela contendo elementos |
| index1 | number | Não | — | Índice do primeiro elemento |
| index2 | number | Não | — | Índice do segundo elemento |

#### Exemplo
```lua
local items = {"A", "B", "C"}
swapTableElements(items, 1, 3)
-- items agora é {"C", "B", "A"}
```

---

### showSkillLevel

Mostra nível ou percentual de uma skill.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| skill | string | Não | — | Nome da skill |
| type | string | Não | — | 'percent' ou 'level' |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| number | Valor da skill |

#### Exemplo
```lua
local swordPercent = showSkillLevel("Sword", "percent")
local swordLevel = showSkillLevel("Sword", "level")
print("Espada: " .. swordLevel .. " (" .. swordPercent .. "%)")
```

---

### calcStamina

Calcula a stamina atual do jogador.

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| string | Stamina formatada "HH:MM" |
| string | Percentual entre parênteses |

#### Exemplo
```lua
local stamTime, stamPercent = calcStamina()
print("Stamina: " .. stamTime .. " " .. stamPercent)
```

---

### itemAmount

Conta a quantidade de um item específico no inventário.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| id | number | Não | — | ID do item |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| number | Quantidade de itens |

#### Exemplo
```lua
local goldCount = itemAmount(3031)
print("Gold coins: " .. goldCount)
```

---

### getFirstNumberInText

Extrai o primeiro número de um texto.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| text | string | Não | — | Texto para analisar |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| number | Primeiro número encontrado ou nil |

#### Exemplo
```lua
local num = getFirstNumberInText("Player lost 150 hitpoints")
-- num = 150
```

---

### isValidSize

Valida se um tamanho é válido (números positivos).

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| size | table | Não | — | Tamanho com campos x e y |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se válido |

#### Exemplo
```lua
local valid = isValidSize({x = 100, y = 50})
-- valid = true
```

---

### extractSpecificTextInString

Extrai texto específico entre dois padrões em uma string.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| str | string | Não | — | String de entrada |
| startPattern | string | Não | — | Padrão de início |
| endPattern | string | Não | — | Padrão de fim |
| offsetStart | number | Sim | 1 | Offset para início |
| offsetEnd | number | Sim | -1 | Offset para fim |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| string | Substring extraída ou nil |

#### Exemplo
```lua
local text = "Player [John] says: Hello"
local name = extractSpecificTextInString(text, "%[", "%]")
-- name = "John"
```

---

### firstLetterUpper

Capitaliza a primeira letra de uma string.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| str | string | Não | — | String de entrada |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| string | String com primeira letra maiúscula |

#### Exemplo
```lua
local capitalized = firstLetterUpper("hello world")
-- capitalized = "Hello World"
```

---

### compareLowerStrings

Compara duas strings sem diferenciar maiúsculas/minúsculas.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| str1 | string | Não | — | Primeira string |
| str2 | string | Não | — | Segunda string |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se str2 está dentro de str1 |

#### Exemplo
```lua
local contains = compareLowerStrings("Hello World", "world")
-- contains = true
```

---

### generateRandomString

Gera uma string aleatória.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| length | number | Sim | 10 | Comprimento da string |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| string | String aleatória |

#### Exemplo
```lua
local randomId = generateRandomString(8)
-- randomId = "aB3dEfG7"
```

---

### doFormatTime

Formata um valor de tempo em string legível.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| time | number | Não | — | Valor de tempo |
| millis | boolean | Sim | false | Se o tempo está em milissegundos |
| mode | string | Sim | "auto" | Modo: "ms", "s", "m:s", "h:m:s", "d:h:m:s", "auto" |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| string | Tempo formatado |

#### Exemplo
```lua
local formatted = doFormatTime(3665, false, "h:m:s")
-- formatted = "1h 1m 5s"

local autoFormatted = doFormatTime(125, true)
-- autoFormatted = "125ms"
```

---

### automaticPercentage

Calcula uma porcentagem automática baseada no número de criaturas na área.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| multiplier | number | Sim | 5 | Multiplicador por criatura |
| basePercentage | number | Sim | 40 | Porcentagem base |
| typeCreature | string/boolean | Sim | — | Tipo de criatura para contar |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| number | Porcentagem calculada |

#### Exemplo
```lua
-- Calcular porcentagem de cura baseada em players próximos
local healPercent = automaticPercentage(5, 40, "player")
```

---

### doDownloadImage

Baixa uma imagem de uma URL e atualiza um widget.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| imageUrl | string | Não | — | URL da imagem |
| loader | table | Não | — | Widget para atualizar |
| type | string | Não | — | Tipo: "icon" ou "image" |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se bem sucedido |

#### Exemplo
```lua
doDownloadImage("https://example.com/icon.png", widget, "icon")
```

---

### doCast

Conjura um feitiço com verificações de segurança contra spam.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| spell | string | Não | — | Nome do feitiço |
| once | boolean | Sim | — | Se true, conjura apenas se não estiver parado |
| callback | function | Sim | nil | Callback para sobrescrever needStop |

#### Exemplo
```lua
-- Conjurar feitiço com segurança
doCast("exori", true, function(needStop)
    return needStop or mana() < 100
end)

-- Conjurar toda vez que possível
doCast("utevo lux", false)
```

#### Notas
- Previne spam de feitiços (cooldown de 200ms)
- Rastreia contagem e tempo de conjurações
- Permite callback para lógica personalizada

---

### getAttackerName

Obtém o nome do último jogador que atacou o jogador local.

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| string | Nome do atacante ou nil |

#### Exemplo
```lua
local attacker = getAttackerName()
if attacker then
    print("Atacado por: " .. attacker)
end
```

---

### getAttackersCount

Conta o número de jogadores atacando o jogador local.

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| number | Contagem de atacantes |

#### Exemplo
```lua
local attackerCount = getAttackersCount()
if attackerCount > 0 then
    print(attackerCount .. " jogadores atacando")
end
```

---

### getTabs

Obtém informações sobre todas as abas disponíveis.

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Lista de abas com nome e conteúdo |

#### Exemplo
```lua
local tabs = getTabs()
for _, tab in ipairs(tabs) do
    print("Tab: " .. tab.name)
end
```

---

### cipherBot.getMacroStorage

Obtém ou cria storage específico para uma macro.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| macroName | string | Não | — | Nome da macro |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Storage da macro |

#### Exemplo
```lua
local macroStorage = cipherBot.getMacroStorage("AutoHeal")
macroStorage.delay = 200
cipherBot.doSaveFile()
```

---

### cipherBot.createMacroSettings

Cria uma janela de configurações para macro com campos personalizáveis.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| macroName | string | Não | — | Nome da macro |
| options | table | Sim | {} | Opções de configuração |

#### Opções
| Campo | Tipo | Descrição |
| :--- | :--- | :--- |
| storageAlias | string | Alias para storage |
| order | table | Ordem dos campos |
| hideName | boolean | Esconder campo nome |
| hideKey | boolean | Esconder campo tecla |
| hideDelay | boolean | Esconder campo delay |
| hideTab | boolean | Esconder campo aba |
| hideIcon | boolean | Esconder campo ícone |
| extraFields | table | Campos extras |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Janela de configurações |

#### Exemplo
```lua
local settingsWindow = cipherBot.createMacroSettings("AutoHeal", {
    order = {"name", "delay", "tab"},
    extraFields = {
        {
            type = "scrollbar",
            id = "healPercent",
            storageKey = "healPercent",
            label = "Percentual de Cura",
            min = 10,
            max = 100,
            default = 70
        }
    }
})
```

---

### cipherBot.getMacroName

Obtém o nome configurado de uma macro.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| macroName | string | Não | — | Nome da macro |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| string | Nome da macro ou string vazia |

---

### cipherBot.getMacroKey

Obtém a tecla configurada de uma macro.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| macroName | string | Não | — | Nome da macro |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| string | Tecla da macro ou string vazia |

---

### cipherBot.getMacroDelay

Obtém o delay configurado de uma macro.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| macroName | string | Não | — | Nome da macro |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| number | Delay da macro ou 100 |

---

### cipherBot.getMacroTab

Obtém a aba configurada de uma macro.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| macroName | string | Não | — | Nome da macro |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| string | Aba da macro ou "Main" |

---

### cipherBot.getMacroIcon

Obtém se a macro tem ícone configurado.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| macroName | string | Não | — | Nome da macro |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se tem ícone |

---

### cipherBot.isScriptEnabled

Verifica se um script está ativado.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| fileName | string | Não | — | Nome do arquivo de script |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se ativado |

#### Exemplo
```lua
if cipherBot.isScriptEnabled("autoHeal.lua") then
    print("AutoHeal está ativo")
end
```

---

### cipherBot.registerMacroSettings

Registra opções de configuração para uma macro.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| macroName | string | Não | — | Nome da macro |
| options | table | Sim | {} | Opções de configuração |

#### Exemplo
```lua
cipherBot.registerMacroSettings("AutoHeal", {
    order = {"name", "delay"},
    hideIcon = true
})
```

---

### cipherBot.setMacroName

Define o nome de uma macro.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| macroName | string | Não | — | Nome da macro |
| name | string | Não | — | Novo nome |

---

### cipherBot.setMacroKey

Define a tecla de uma macro.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| macroName | string | Não | — | Nome da macro |
| key | string | Não | — | Nova tecla |

---

### cipherBot.setMacroDelay

Define o delay de uma macro.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| macroName | string | Não | — | Nome da macro |
| delay | number | Não | — | Novo delay |

---

### cipherBot.setMacroTab

Define a aba de uma macro.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| macroName | string | Não | — | Nome da macro |
| tab | string | Não | — | Nova aba |

---

### cipherBot.setMacroIcon

Define se uma macro tem ícone.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| macroName | string | Não | — | Nome da macro |
| icon | boolean | Não | — | true para ícone |

---

### cipherBot.deleteMacro

Deleta uma macro do storage.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| macroName | string | Não | — | Nome da macro |

---

### cipherBot.listMacros

Lista todas as macros registradas.

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Nomes das macros |

#### Exemplo
```lua
local macros = cipherBot.listMacros()
for _, name in ipairs(macros) do
    print("Macro: " .. name)
end
```

---

### cipherBot.resetMacro

Reseta todas as configurações de uma macro.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| macroName | string | Não | — | Nome da macro |

---

### cipherBot.cloneMacro

Clona as configurações de uma macro para outra.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| originalName | string | Não | — | Nome da macro original |
| newName | string | Não | — | Nome da nova macro |

---

### cipherBot.macroExists

Verifica se uma macro existe.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| macroName | string | Não | — | Nome da macro |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se existe |

---

### cipherBot.updateMacro

Atualiza múltiplas propriedades de uma macro.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| macroName | string | Não | — | Nome da macro |
| data | table | Não | — | Dados para atualizar |

#### Exemplo
```lua
cipherBot.updateMacro("AutoHeal", {
    name = "Cura Automática",
    delay = 250,
    tab = "Healing"
})
```

---

### cipherBot.macro

Cria uma macro com gerenciamento avançado.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| timeout | number | Não | — | Intervalo de execução |
| name | string | Sim | "" | Nome da macro |
| hotkey | string | Sim | "" | Tecla de atalho |
| callback | function | Não | — | Função de callback |
| parent | table | Sim | context.panel | Widget pai |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Objeto macro |

#### Exemplo
```lua
local myMacro = cipherBot.macro(100, "AutoAttack", "Ctrl+A", function()
    if target() then
        attack(target())
    end
end)

-- Controlar macro
myMacro.setOn()
myMacro.setOff()
myMacro.toggle()
```

---

### cipherBot.setDefaultTab

Define a aba padrão para o script atual.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| tabName | string | Não | — | Nome da aba |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se bem sucedido |

#### Exemplo
```lua
-- Definir aba no início do script
cipherBot.setDefaultTab("Healing")
```

---

### cipherBot.getCurrentTab

Obtém o nome da aba ativa atual.

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| string | Nome da aba ou nil |

---

### cipherBot.listTabs

Lista todas as abas disponíveis.

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Nomes das abas |

---

### cipherBot.tabExists

Verifica se uma aba existe.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| tabName | string | Não | — | Nome da aba |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se existe |

---

### insertSpellList

Insere uma lista de feitiços em um widget de lista.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| spellList | table | Não | — | Widget de lista |
| storageData | table | Não | — | Dados de storage |
| visibilityConfig | table | Sim | nil | Configuração de visibilidade |
| customText | string/function | Sim | nil | Texto personalizado |
| customTooltip | string/function | Sim | nil | Tooltip personalizado |
| onDoubleClickCallback | function | Sim | nil | Callback para duplo clique |

#### Exemplo
```lua
insertSpellList(spellListWidget, cipherBot.storage.spells, {
    show = {"enabled", "remove"},
    hide = {"timeSpellEnabled"}
}, function(entry)
    return "Spell: " .. entry.name
end)
```

---

## 🎯 Icon Library

### cipherBot.Icon.create

Cria um ícone interativo na tela do jogo.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| id | string | Não | — | ID único do ícone |
| options | table | Não | — | Opções do ícone |
| callback | function | Não | — | Função de callback |

#### Opções
| Campo | Tipo | Descrição |
| :--- | :--- | :--- |
| item | table/number | Item para exibir |
| image | string | Imagem local |
| imageUrl | string | URL da imagem |
| outfit | table | Outfit de criatura |
| creatureId | number | ID da criatura |
| text | string | Texto do ícone |
| x | number | Posição X (0.0-1.0) |
| y | number | Posição Y (0.0-1.0) |
| hotkey | string | Tecla de atalho |
| switchable | boolean | true | Se pode alternar |
| movable | boolean | true | Se pode mover |
| phantom | boolean | false | Se é fantasma |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| table | Widget do ícone |

#### Exemplo
```lua
-- Ícone de item
cipherBot.Icon.create("healPotion", {
    item = {id = 7618, count = 10},
    text = "Heal",
    x = 0.1,
    y = 0.5,
    hotkey = "F1"
}, function(widget, isOn)
    if isOn then
        useItem(7618)
    end
end)

-- Ícone de outfit
cipherBot.Icon.create("playerTracker", {
    outfit = {type = 128, head = 94, body = 113, legs = 115, feet = 115},
    text = "Track"
}, trackPlayer)
```

---

### cipherBot.Icon.changeVisibility

Altera a visibilidade de um ícone.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| id | string | Não | — | ID do ícone |
| hide | boolean | Não | — | true para esconder |

#### Exemplo
```lua
cipherBot.Icon.changeVisibility("healPotion", true) -- Esconder
cipherBot.Icon.changeVisibility("healPotion", false) -- Mostrar
```

---

### cipherBot.Icon.setCallback

Define um novo callback para um ícone.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| id | string | Não | — | ID do ícone |
| newCallback | function | Não | — | Novo callback |

#### Exemplo
```lua
cipherBot.Icon.setCallback("healPotion", function(widget, status)
    if status then
        say("exura vita")
    end
end)
```

---

### cipherBot.Icon.setText

Altera o texto de um ícone.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| id | string | Não | — | ID do ícone |
| newText | string | Não | — | Novo texto |

#### Exemplo
```lua
cipherBot.Icon.setText("healPotion", "Strong Heal")
```

---

### cipherBot.Icon.setColor

Altera a cor do texto de um ícone.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| id | string | Não | — | ID do ícone |
| newText | string | Não | — | Nova cor (HEX) |

#### Exemplo
```lua
cipherBot.Icon.setColor("healPotion", "#FF0000") -- Vermelho
```

---

### cipherBot.Icon.setItem

Altera o item exibido em um ícone.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| id | string | Não | — | ID do ícone |
| item | table/number | Não | — | Novo item |

#### Exemplo
```lua
-- Mudar para mana potion
cipherBot.Icon.setItem("healPotion", {id = 7620, count = 5})

-- Apenas mudar ID
cipherBot.Icon.setItem("healPotion", 268)
```

---

### cipherBot.Icon.setOutfit

Altera o outfit exibido em um ícone.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| id | string | Não | — | ID do ícone |
| outfit | table | Não | — | Novo outfit |

#### Exemplo
```lua
cipherBot.Icon.setOutfit("playerTracker", {
    type = 130,
    head = 95,
    body = 114,
    legs = 116,
    feet = 116
})
```

---

### cipherBot.Icon.setOn

Ativa um ícone.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| id | string | Não | — | ID do ícone |
| on | boolean | Não | — | Estado |

#### Exemplo
```lua
cipherBot.Icon.setOn("healPotion", true)
```

---

### cipherBot.Icon.setOff

Desativa um ícone.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| id | string | Não | — | ID do ícone |
| on | boolean | Não | — | Estado |

#### Exemplo
```lua
cipherBot.Icon.setOff("healPotion", true)
```

---

### cipherBot.Icon.isOn

Verifica se um ícone está ativo.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| id | string | Não | — | ID do ícone |

#### Retorno
| Tipo | Descrição |
| :--- | :--- |
| boolean | true se ativo |

#### Exemplo
```lua
if cipherBot.Icon.isOn("healPotion") then
    print("Ícone de cura ativo")
end
```

---

### cipherBot.Icon.remove

Remove um ícone da tela.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| id | string | Não | — | ID do ícone |

#### Exemplo
```lua
cipherBot.Icon.remove("healPotion")
```

---

## 🔔 Alert Library

### cipherBot.showAlert

Exibe uma notificação temporária na tela.

#### Parâmetros
| Parâmetro | Tipo | Opcional | Padrão | Descrição |
| :--- | :--- | :--- | :--- | :--- |
| params | table | Não | — | Parâmetros do alerta |

#### Estrutura de `params`
| Campo | Tipo | Padrão | Descrição |
| :--- | :--- | :--- | :--- |
| title | string | "Alert" | Título do alerta |
| message | string | "" | Mensagem do alerta |
| duration | number | 2000 | Duração em milissegundos |
| outDuration | number | 500 | Duração da animação de saída |
| colorBorder | string | "#9D4EDD" | Cor da borda |
| colorTitle | string | "#9D4EDD" | Cor do título |
| colorText | string | "#E0E0E0" | Cor do texto |

#### Exemplo
```lua
-- Alert simples
cipherBot.showAlert({
    title = "Aviso",
    message = "Mana baixa!",
    duration = 1500
})

-- Alert personalizado
cipherBot.showAlert({
    title = "Perigo",
    message = "Vida crítica! Usando potion...",
    duration = 3000,
    colorBorder = "#FF0000",
    colorTitle = "#FF5555",
    colorText = "#FFFFFF"
})
```

#### Notas
- Tamanho automático baseado no comprimento do texto
- Barra de progresso mostra tempo restante
- Animações de fade in/out suportadas
- Múltiplos alerts são enfileirados

---

## 🎯 Exemplos Avançados

### Sistema de Auto Heal Completo
```lua
if (not cipherBot) then return end

-- Definir aba padrão
cipherBot.setDefaultTab("Healing")

-- Criar janela de configurações
local window = cipherBot.UI.create("Auto Heal", 350, 400)

-- Seção de configurações básicas
local basicSection = cipherBot.UI.section("Configurações Básicas", window.mainPanel)

cipherBot.UI.switch("autoHeal", "enabled", "Ativar Auto Heal", false, basicSection)
cipherBot.UI.scrollbar("autoHeal", "healthPercent", "Curar abaixo de %", 10, 100, 50, basicSection, nil, {
    format = "percent"
})

-- Seção de itens de cura
local itemsSection = cipherBot.UI.section("Itens de Cura", window.mainPanel)

cipherBot.UI.item("autoHeal", "healthPotion", "Poção de Vida", 7618, itemsSection)
cipherBot.UI.scrollbar("autoHeal", "potionHealth", "Vida para poção %", 10, 100, 30, itemsSection, nil, {
    format = "percent"
})

-- Seção de feitiços
local spellsSection = cipherBot.UI.section("Feitiços", window.mainPanel)

cipherBot.UI.switch("autoHeal", "useExura", "Usar Exura", true, spellsSection)
cipherBot.UI.scrollbar("autoHeal", "exuraHealth", "Vida para Exura %", 10, 100, 70, spellsSection, nil, {
    format = "percent"
})

-- Macro de execução
cipherBot.macro(100, "AutoHeal", "Ctrl+H", function()
    if not cipherBot.storage.autoHeal.enabled then return end
    
    local hpPercent = healthpercent()
    local player = g_game.getLocalPlayer()
    
    -- Usar poção de vida
    if hpPercent <= cipherBot.storage.autoHeal.potionHealth then
        local potionId = cipherBot.storage.autoHeal.healthPotion
        if itemAmount(potionId) > 0 then
            useItem(potionId)
            return
        end
    end
    
    -- Usar feitiço
    if cipherBot.storage.autoHeal.useExura and hpPercent <= cipherBot.storage.autoHeal.exuraHealth then
        if mana() >= 20 then
            doCast("exura", true)
        end
    end
end)
```

### Sistema de Alerta de PZ
```lua
if (not cipherBot) then return end

-- Widget de status PZ
local pzWidget = cipherBot.Widget.create("pzStatus", "Fora de PZ", "#00FF00")

-- Macro para monitorar PZ
cipherBot.macro(500, "PZMonitor", "", function()
    local player = g_game.getLocalPlayer()
    if not player then return end
    
    if player:isInPz() then
        cipherBot.Widget.changeText("pzStatus", "EM PZ!", "#FF0000")
        cipherBot.Widget.changeColor("pzStatus", "#FF0000")
        
        -- Alert sonoro visual
        cipherBot.showAlert({
            title = "ALERTA PZ",
            message = "Você está em Protected Zone!",
            duration = 3000,
            colorBorder = "#FF0000",
            colorTitle = "#FF5555"
        })
    else
        cipherBot.Widget.changeText("pzStatus", "Fora de PZ", "#00FF00")
        cipherBot.Widget.changeColor("pzStatus", "#00FF00")
    end
end)
```

### Sistema de Rotação de Feitiços
```lua
if (not cipherBot) then return end

-- Configurar aba
cipherBot.setDefaultTab("Rotation")

-- Criar lista de feitiços
cipherBot.storage.spellRotation = cipherBot.storage.spellRotation or {
    spells = {
        {name = "exori", enabled = true, mana = 20},
        {name = "exori gran", enabled = true, mana = 110},
        {name = "exori mort", enabled = false, mana = 20}
    }
}

-- Janela de configuração
local window = cipherBot.UI.create("Spell Rotation", 300, 350)
local spellList = cipherBot.UI.scrollablePanel("Feitiços", window.mainPanel)

-- Função para inserir lista
local function refreshSpellList()
    insertSpellList(spellList.list, cipherBot.storage.spellRotation, {
        show = {"enabled", "remove"}
    }, function(entry)
        return entry.name .. " (" .. entry.mana .. " mana)"
    end)
end

-- Botão para adicionar feitiço
cipherBot.UI.button("Adicionar Feitiço", function()
    local spellName = "exori"
    table.insert(cipherBot.storage.spellRotation.spells, {
        name = spellName,
        enabled = true,
        mana = 20
    })
    cipherBot.doSaveFile()
    refreshSpellList()
end, window.mainPanel)

-- Macro de rotação
cipherBot.macro(1000, "SpellRotation", "", function()
    if not target() then return end
    
    for _, spell in ipairs(cipherBot.storage.spellRotation.spells) do
        if spell.enabled and mana() >= spell.mana then
            doCast(spell.name, true)
            break
        end
    end
end)

-- Inicializar lista
refreshSpellList()
```

---

## ❓ Perguntas Frequentes

---

## 🔗 Referências


---
