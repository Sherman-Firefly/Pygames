import pygame

pygame.init()

white=(255,255,255)

clock=pygame.time.Clock()

display_surface=pygame.display.set_mode((500,500))
pygame.display.set_caption("Display Text in Pygame")

pygame.display.set_caption('image')
image=pygame.image.load('LAFLT1.png')

font = pygame.font.Font(None, 36) 

text = font.render("Hello, Pygame! Submarine pic :)", True, white)
text_rect = text.get_rect(center=(500 // 2, 10))

DEFAULT_IMAGE_SIZE=(500,500)
image=pygame.transform.scale(image,DEFAULT_IMAGE_SIZE)

DEFAULT_IMAGE_POSITION=(0,0)

while True:
    display_surface.fill(white)
    display_surface.blit(image, DEFAULT_IMAGE_POSITION)
    for event in pygame.event.get():
        if event.type==pygame.QUIT:
            pygame.quit()
    display_surface.blit(text, text_rect)
    pygame.display.flip()
    clock.tick(30)