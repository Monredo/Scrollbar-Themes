<p>
<img src="https://raw.githubusercontent.com/Monredo/scrolltello/main/scrolltello.png">
</p>

Lees in [English](https://github.com/Monredo/scrolltello/blob/main/README.md) | [Español](https://github.com/Monredo/scrolltello/blob/main/extras/README_ES.md) | [Italiano](https://github.com/Monredo/scrolltello/blob/main/extras/README_IT.md)

Scrolltello - Een gekleurde schuifbalk met standaardthema's die mensen kunnen gebruiken.
###### Probleembeschrijving
De `::webkit-scrollbar-button:disabled` werkt niet voor deze status.
# Voorbeeld
Bijvoorbeeld als volgt:
```css
::-webkit-scrollbar {
  width: 17px;
  height: 17px;
}

::-webkit-scrollbar-track {
  background: #f1f1f1; 
}

::-webkit-scrollbar-thumb {
  background-color: #c1c1c1;
  border: 2px solid #f1f1f1;
}

::-webkit-scrollbar-thumb:hover {
  background-color: #a8a8a8;
}

::-webkit-scrollbar-thumb:active {
  background-color: #787878;
}

::-webkit-scrollbar-button {
  background-color: #f1f1f1;
  background-repeat: no-repeat;
  background-size: 7px;
  background-position: center;
  height: 17px;
  width: 17px;
}

::-webkit-scrollbar-button:hover {
  background-color: #d2d2d2;
  background-repeat: no-repeat;
  background-size: 7px;
  background-position: center;
  height: 17px;
  width: 17px;
}

::-webkit-scrollbar-button:active {
  background-color: #787878;
  background-repeat: no-repeat;
  background-size: 7px;
  background-position: center;
  height: 17px;
  width: 17px;
}

::-webkit-scrollbar-button:vertical:decrement {
  background-image: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100' fill='%23505050'><polygon points='50,30 100,80 0,80'/></svg>");
}

::-webkit-scrollbar-button:vertical:increment {
  background-image: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100' fill='%23505050'><polygon points='0,15 100,15 50,75'/></svg>");
}

::-webkit-scrollbar-button:horizontal:decrement {
  background-image: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100' fill='%23505050'><polygon points='15,50 75,100 75,0'/></svg>");
}

::-webkit-scrollbar-button:horizontal:increment {
  background-image: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100' fill='%23505050'><polygon points='15,0 15,100 75,50'/></svg>");
}

::-webkit-scrollbar-button:vertical:decrement:active {
  background-image: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100' fill='%23ffffff'><polygon points='50,30 100,80 0,80'/></svg>");
}

::-webkit-scrollbar-button:vertical:increment:active {
  background-image: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100' fill='%23ffffff'><polygon points='0,15 100,15 50,75'/></svg>");
}

::-webkit-scrollbar-button:horizontal:decrement:active {
  background-image: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100' fill='%23ffffff'><polygon points='15,50 75,100 75,0'/></svg>");
}

::-webkit-scrollbar-button:horizontal:increment:active {
  background-image: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100' fill='%23ffffff'><polygon points='15,0 15,100 75,50'/></svg>");
}

::-webkit-scrollbar-corner {
  background-color: #dddddd;
}
```
# Schuifbalkkiezers
Voor webkit-browsers kunt u de volgende pseudo-elementen gebruiken om de schuifbalk van de browser aan te passen:
- `::-webkit-scrollbar` De schuifbalk.
- `::-webkit-scrollbar-button` De knoppen op de scrollbar (pijlen die naar boven en naar beneden wijzen).
- `::-webkit-scrollbar-thumb` De versleepbare schuifgreep.
- `::-webkit-scrollbar-track` De track (voortgangsbalk) van de schuifbalk.
- `::-webkit-scrollbar-track-piece` De baan (voortgangsbalk) wordt NIET afgedekt door het handvat.
- `::-webkit-scrollbar-corner` De benedenhoek van de schuifbalk, waar zowel horizontale als verticale schuifbalken samenkomen.
- `::-webkit-resizer` De versleepbare formaatgreep die in de benedenhoek van sommige elementen verschijnt.
