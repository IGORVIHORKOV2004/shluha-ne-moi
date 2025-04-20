import pygame

def draw_circle(sc, x,y,size):
    size=200
    a=  x *    size    +   0.5    *   size
    b=  y *    size    +   0.5 *  size
    pygame.draw.circle(sc,(0,0,255),(a,b),100)

def draw_cross(sc, x,y,size):
    size=200
    a=x*200
    b=y*200
    a1= a+200
    b1=b+200
    pygame.draw.line(sc,(255,0,0,),(a,b),(a1,b1),5)
    pygame.draw.line(sc,(255,0,0,),(a1,b),(a,b1),5)
window_size = (600, 600)
screen = pygame.display.set_mode(window_size)  # создание экрана(окна) с размера 300x300
screen.fill((255, 255, 255))
pygame.draw.line(screen, (0,0,0), (0, 200), (600, 200), 5)
pygame.draw.line(screen, (0,0,0), (0, 400), (600, 400), 5)
pygame.draw.line(screen, (0,0,0), (200, 0), (200, 600), 5)
pygame.draw.line(screen, (0,0,0), (400,0), (400, 600), 5)
clock = pygame.time.Clock()  # создание игровово таймера
draw_circle(screen,1,2,200)
draw_cross(screen,1,1,200)


while True:  # игрововй таймер
    clock.tick(40)  # частота обновления таймераааааа
    for event in pygame.event.get():  # проходимся по событиям
        if event.type == pygame.QUIT:  # если нажали на крестик
            pygame.QUIT()  # выйти из ГОЙДА
    pygame.display.update()  # ОБНОВЛЕНИЕ ДИСПЛЕЯ
