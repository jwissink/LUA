# LUA point and click adventure
In deze repository staat een engine gemaakt in C++ waarin de gameplay geprogrammeerd kan worden in LUA.
Om hiermee aan de slag te gaan is er het volgende stappenplan:
1. Download repository (rechts boven staat download of via je shell: git clone https://github.com/jwissink/LUA/)
2. Open `Script.LUA` en lees de text en functies
3. Open `SFMLCore.exe` en bekijk wat de code doet
4. Maak het bestand `Script.lua` leeg
5. Maak je eigen gameplay met de volgende functies
* setBackground

   Zet de achtergond naar een plaatje in de Textures folder

* createButton 

   Voegt een knop toe aan het spel

* createTextfield

   Voegt een textvlak toe aan het spel

* CLS

   Maakt het scherm leeg

* exitGame

   Sluit het spel

* playSound

   Speelt een geluid uit de Sounds folder (wav)

* playMusic

   Speelt muziek uit de Music folder (wav)

## uitleg
Om de functie aan te roepen moeten er vaak argumenten mee gegeven worden. Zoals bijvoorbeeld welk plaatje weer gegeven moet worden of welke muziek afgespeeld moet worden. De argumenten in code worden mee gegeven met ( ).

### voorbeelden:
* `setBackground("myAmazingBackground.jpg)`
* `playMusic("someCoolMusic.wav)`
* `playSound("myShootingSound.wav)`

#### Tutorial
Deze tutorial gaat ervan uit dat je de repository al hebt gedownload en uitgepakt op je laptop.

Hier staat een stappenplan om een begin te maken:
1. Open het bestand `Script.lua` met een text editor zoals Notepad++ of visual studio en zorg ervoor dat deze compleet leeg is.
2. voeg het volgende stukje code toe aan je `Script.lua`:
```lua
function story(aName)
    if(aName == "start") then
        playMusic("background.wav")
    end
end
```
Het spel start altijd bij de functie `story` met als argument `start`
3. 
