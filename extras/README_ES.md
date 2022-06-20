<p>
<img src="https://raw.githubusercontent.com/Monredo/scrolltello/main/scrolltello.png">
</p>

Scrolltello - Barras de desplazamiento de colores con temas predeterminados para que la gente los use.
###### Descripción del problema
El `::webkit-scrollbar-button:disabled` no funciona para este estado.
# Ejempla
Por ejempla, así:
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
# Selectores de la barra de desplazamiento
Para navegadores webkit, puede usar los siguientes pseudo elementos para personalizar la barra de desplazamiento del navegador:
- `::-webkit-scrollbar` La barra de desplazamiento.
- `::-webkit-scrollbar-button` Los botones de la barra de desplazamiento (flechas que apuntan hacia arriba y hacia abajo).
- `::-webkit-scrollbar-thumb` El controlador de desplazamiento arrastrable.
- `::-webkit-scrollbar-track` La pista (barra de progreso) de la barra de desplazamiento.
- `::-webkit-scrollbar-track-piece` El pista (barra de progreso) NO está cubierta por el mango.
- `::-webkit-scrollbar-corner` La esquina inferior de la barra de desplazamiento, donde se encuentran las barras de desplazamiento horizontal y vertical.
- `::-webkit-resizer` La controlador de cambio de tamaño arrastrable que aparece en la esquina inferior de algunos elementos.
