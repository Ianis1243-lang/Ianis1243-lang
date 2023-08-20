I am learning to code Python and now going to Pygame. Here is some code that I made:
import pygame

pygame.init()

screen_width = 800
screen_height = 600
screen = pygame.display.set_mode((screen_width, screen_height))
pygame.display.set_caption("Pingu Pygame")

running = True
while running:
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            running = False

    screen.fill((255, 255, 255))

    pygame.draw.rect(screen, (0, 0, 255), (200, 200, 50, 50))

    pygame.display.update()

pygame.quit()


Python:


import time

print("Hello!")


time.sleep(1)

answer = input("Do you want to make pancakes? (yes/no): ")

if answer.lower() == "yes":
    amount_of_eggs = int(input("Great! How many eggs do you have?"))
    amount_of_flour = int(input("How many cups of flour do you have?"))
    amount_of_baking_powder = int(input("How many teaspoons of baking powder do you have?"))
    amount_of_sugar = int(input("How many tablespoons of sugar do you have?"))
    amount_of_salt = int(input("How many teaspoons of salt do you have?"))
    amount_of_milk = int(input("How many cups of milk do you have?")) 
    amount_of_oil = int(input("How many tablespoons of oil do  you have?"))

    minimum_eggs_required = 1  
    minimum_flour_required = 1
    minimum_baking_powder_required = 1
    minimum_sugar_required = 1
    minimum_salt_required = 1
    minimum_milk_required = 1
    minimum_oil_required = 1

    if (amount_of_eggs >= minimum_eggs_required and
        amount_of_flour >= minimum_flour_required and
        amount_of_baking_powder >= minimum_baking_powder_required and
        amount_of_sugar >= minimum_sugar_required and
        amount_of_salt >= minimum_salt_required and
        amount_of_milk >= minimum_milk_required and
        amount_of_oil >= minimum_oil_required):
        print("You have enough ingredients to make pancakes!")
    else:
        print("Sorry, you don't have enough ingredients to make pancakes.")
else:
    print("Goodbye!")
  
  
input("Press Enter to exit...")
