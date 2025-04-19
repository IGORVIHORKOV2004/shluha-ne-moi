import pygame

pygame.init()
window_size = (800, 800)
screen = pygame.display.set_mode(window_size)  # создание экрана(окна) с размера 300x300
screen.fill((255, 255, 255))
pygame.draw.line(screen, (0,0,0), (0, 50), (800, 50), 5)
pygame.draw.line(screen, (0,0,0), (0, 150), (800, 150), 5)
pygame.draw.line(screen, (0,0,0), (0, 250), (800, 250), 5)
pygame.draw.line(screen, (0,0,0), (0, 350), (800, 350), 5)
pygame.draw.line(screen, (0,0,0), (0, 450), (800, 450), 5)
pygame.draw.line(screen, (0,0,0), (0, 550), (800, 550), 5)
pygame.draw.line(screen, (0,0,0), (0, 650), (800, 650), 5)
pygame.draw.line(screen, (0,0,0), (0, 750), (800, 750), 5)
pygame.draw.line(screen, (0,0,0), (0, 800), (800, 800), 5)
pygame.draw.line(screen, (0,0,0), (50, 0), (50, 800), 5)
pygame.draw.line(screen, (0,0,0), (150,0), (150, 800), 5)
pygame.draw.line(screen, (0,0,0), (250, 0), (250, 800), 5)
pygame.draw.line(screen, (0,0,0), (350, 0), (350, 800), 5)
pygame.draw.line(screen, (0,0,0), (450, 0), (450, 800), 5)
pygame.draw.line(screen, (0,0,0), (550, 0), (550, 800), 5)
pygame.draw.line(screen, (0,0,0), (650, 0), (650, 800), 5)
pygame.draw.line(screen, (0,0,0), (750, 0), (750, 800), 5)
pygame.draw.line(screen, (0,0,0), (800, 0), (800, 800), 5)
clock = pygame.time.Clock()  # создание игровово таймера


while True:  # игрововй таймер
    clock.tick(40)  # частота обновления таймераааааа
    for event in pygame.event.get():  # проходимся по событиям
        if event.type == pygame.QUIT:  # если нажали на крестик
            pygame.QUIT()  # выйти из ГОЙДА
    pygame.display.update()  # ОБНОВЛЕНИЕ ДИСПЛЕЯ
