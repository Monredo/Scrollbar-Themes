# scrollbar-themes
Scrollbar themes - Una barra di scorrimento colorata con temi predefiniti che le persone possono utilizzare.
###### Descrizione del problema
Il `::webkit-scrollbar-button:disabled` non funziona per questo stato.
# Esempio
Ad esempio, in questo modo:
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
# Selettori della barra di scorrimento
Per i browser webkit, puoi utilizzare i seguenti pseudo elementi per personalizzare la barra di scorrimento del browser:
- `::-webkit-scrollbar` La barra di scorrimento.
- `::-webkit-scrollbar-button` I pulsanti sulla barra di scorrimento (frecce rivolte verso l'alto e verso il basso).
- `::-webkit-scrollbar-thumb` La maniglia di scorrimento trascinabile.
- `::-webkit-scrollbar-track` La traccia (barra di avanzamento) della barra di scorrimento.
- `::-webkit-scrollbar-track-piece` La traccia (barra di avanzamento) NON è coperta dalla maniglia.
- `::-webkit-scrollbar-corner` L'angolo inferiore della barra di scorrimento, dove si incontrano sia la barra di scorrimento orizzontale che quella verticale.
- `::-webkit-resizer` La maniglia di ridimensionamento trascinabile che appare nell'angolo inferiore di alcuni elementi.
