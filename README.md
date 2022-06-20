# scrollbar-themes
Scrollbar themes - A coloured scrollbars with Default themes for people to use.
###### Problem Description
The `::webkit-scrollbar-button:disabled` doesn't work for this state.
# Example
For example, like this:
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
# Scrollbar Selectors
For webkit browsers, You can use the following pseudo elements to customize the browser's scrollbar:
- `::-webkit-scrollbar` The scrollbar.
- `::-webkit-scrollbar-button` The buttons on the scrollbar (arrows pointing upwards and downwards).
- `::-webkit-scrollbar-thumb` The draggable scrolling handle.
- `::-webkit-scrollbar-track` The track (progress bar) of the scrollbar.
- `::-webkit-scrollbar-track-piece` The track (progress bar) NOT covered by the handle.
- `::-webkit-scrollbar-corner` The bottom corner of the scrollbar, where both horizontal and vertical scrollbars meet.
- `::-webkit-resizer` The draggable resizing handle that appears at the bottom corner of some elements.
