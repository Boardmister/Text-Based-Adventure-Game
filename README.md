# Text-Based-Adventure-Game
Create a simple text-based adventure game using Python.
import time

def introduction():
    print("Welcome to the Adventure Game!")
    time.sleep(1)
    print("You find yourself in a mysterious place.")
    time.sleep(1)

def make_choice():
    choice = input("Do you want to go left or right? ").lower()
    if choice == 'left':
        print("You chose to go left. You encounter a friendly creature.")
    elif choice == 'right':
        print("You chose to go right. Uh-oh! A trap door opens beneath you.")
    else:
        print("Invalid choice. Try again.")
        make_choice()

introduction()
make_choice()
