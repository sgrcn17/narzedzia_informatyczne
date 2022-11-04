# narzedzia_informatyczne
## projekt MontePyton

#### projekt polega na stworzeniu gry 2D na przedmiot narzędzia informatyczne
#### plik readme został zedytowany przy pomocy [tutoriala:](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

## mechaniki występujące w grze:

#### gra będzie mieć następujące mechaniki: 
* chodzenie
* skakanie
* zbieranie przedmiotów

## używane narzędzia:

#### gra jest robiona przy użyciu następujących narzędzi:
1. Pycharm + pygame
2. git + github
3. discord

## kod głównej pętli gry:
```py
import pygame
from _objects.gameObject import gameObject

background_colour = (234, 212, 252)

screen = pygame.display.set_mode((300, 300))

pygame.display.set_caption('Platformer Game')

screen.fill(background_colour)

pygame.display.flip()

running = True

obiekt = gameObject(1, 1)
print(obiekt.posX)

while running:

    for event in pygame.event.get():

        if event.type == pygame.QUIT:
            running = False
```



| obiekt gry | opis |
| --- | --- |
| gracz | postać którą będzie można się poruszać |
| podłoga | statyczny obiekt po którym będzie można chodzić |
