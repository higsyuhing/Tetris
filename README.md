# Tetris
This is a practice project by Python, which is a Tetris game. 

Library plan, it might use: 
- PyGame
- Pyglet
- PyOpenGL
- others

Framework design: 
1. main
2. openGL init: figure generator, GUI callback (mouse reponse)
3. control and keyboard/mouse responsor
...
a. figure generator
b. GUI callback (mouse reponse)
c. keyboard reponse
d. main state (in game, beginning, end of one game, suspend etc. )
e. game state (current game)
f*. game hardness

Class design: 
GameMain class:{
- figure object (OpenGL)
- Tetris object (not detect input, all by service function)
- main state
- service function: check keyboard, mouse callback
}
Tetris class:{
- game state (map, current)
- hardness and algorithm
- API for change game state
- API for return game figure
}
Figure class:{
- API for showing a figure
- API for returning the GUI callback
}

updated by 05/26/2018, higsyuhing
