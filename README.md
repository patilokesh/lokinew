# lokinew
import pygame
import sys
# this code is about to devolup a chess game with the help of python
# Initialize PyGame.
pygame.display.init()

# Create a screen display window with size 800x600.
screen = pygame.display.set_mode((800, 600), pygame.RESIZABLE)

# Set the title of the window.
pygame.display.set_caption("Chess")

# Create a clock that helps limit the frame rate.
clock = pygame.time.Clock()

# Start the infinite game loop.
while 1:
    # Check events in PyGame to see if the operating system wants us
    # to quit (user closed the window).
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            pygame.quit()
            sys.exit()

    # Ensure that this loop is only running at 120 frames per second.
    clock.tick(120)

    # Fill the frame surface with the color black (RGB values).
    screen.fill((0,0,0))

    # Flip the frame surface to the display.
    pygame.display.flip()
