# nameGenerator.py
This code runs a game that generates a random first and last name for someone
# Author: Ethan Thompson


import random

print("\nWelcome to the Name Generator Machine! We're here for all of your name generation needs!\n")
print("Need a new name because you're running from the government? Maybe you got mad some Yakuza members angry, \n")
print("or maybe you just need a new name for the fun of it, we have you covered\n")
start = input("Would you like to start the machine?\n").upper()

first = ('Aaron', 'Jason', 'Jordan', 'Alex', 'Armani', 'Tony', 'Steve', 'Stephen', 'Paul', 'Alexa', 'Cameron', 'Carter',
         'Tommy', 'Frank', 'David', 'Jimothy', 'Eric', 'Paula', 'Artis', 'Jack', 'Melvin', 'T-Bone', 'J-Money')

last = ('Tomlin', 'Jackson', 'Melvinson', 'Dorman', 'Spengler', 'Rihanna', 'Flenderson', 'Scott', 'Halpert', 'Malone'
                                                                                                             'Korg',
        'SnackGod', 'MonsterTruck', 'YooguiOh', 'Delphine', 'Star', 'Brokauv')

if start == "YES":

    while True:

        random_first = random.choice(first)
        random_last = random.choice(last)

        print("Your new name is:")
        print(random_first + " " + random_last + "\n")
        nextRun = input(
            "Would you like a different name? It's a very small cost of your dignity (Press enter to continue, 'no' to"
            " stop the machine)\n").upper()
        if nextRun == "NO":
            print("Machine function terminated. Thank you for wasting its time\n")
            break





elif start == "NO":

    print("Very well, enjoy your boring name\n")
