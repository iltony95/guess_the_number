#!/usr/bin/env python3

import random

number = random.randint(1, 10)

print("Welcome in this new ADVENTURE!")
name = input("What is your name?")
start_game = input("Hi "+name.upper()+" !\nDo you want to play with me?    [Y/N]")
if start_game == "n":
	print("Why do you launch me?!?    (-_-)'")
while start_game == "y":
	tries = 0
	difficult = int(input("Choise a difficult:\n[0] You have 5 tries.\n[1] You have 3 tries.\n[2] You have 1 try.\n"))
	if difficult == 0:
		tries = 5
	elif difficult == 1:
		tries = 3
	else:
		tries = 1
		
	print("Very cool!! Now i play with you 3:O\nI'm thinking of a number between 1 & 10....")
	while True:
		guess = int(input("Have a guess?"))
		if guess == number:
			print("Good choise guy!    You finish the game with",tries,"tries.")
			start_game = input("Do you want to play again?    [Y/N]")
			break
		else:
			print("Bad choise guy!")
			tries -= 1
			if tries > 0:
				print("You have another",tries,"tries")
			else:
				print("Sorry guy but you finish your try.\nThe number was",number)
				tries = 3
				start_game = input("Do you want to play again?    [Y/N]")
				break
			
