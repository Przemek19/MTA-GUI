# MTA-GUI

System GUI do MTA.

Przykłady:

```lua
GUI = exports["MTA-GUI"] -- Skraca nazwę zmiennej, aby nie pisać za każdym razem np. exports["MTA-GUI"]:setText(...)
window = GUI:createWindow(100, 100, 400, 300) -- Tworzy element GUI (okienko)
GUI:setText(window, "Testowe okienko") -- Nadaje tekst na element
GUI:setFont(window, "Lato", 18, "light") -- Zmienia czcionkę elementu
GUI:setBorderRadius(window, 4) -- Dodaje zaokrąglenia na rogach

addEventHandler("onDXGUIClick", window, function(bttn, state)
  outputChatBox("Klik (" .. bttn .. " | " .. state .. ")")
end)
```
