# Snake-Water-Gun-game

import random

def game( win, lose ):
    if comp == 1:
        if player == "S":
            return None
        elif player == "W":
            return False
        elif player == "G":
            return True
    elif comp == 2:
        if player == "S":
            return "True"
        elif player == "W":
            return None
        elif player == "G":
             return False

    elif comp == 3:
         if player == "S":
              return False
         elif player == "W":
              return True
         elif player == "G":
              return None
comp = random.randint(1, 3)

print("Computer's turn: ")
player = input("Player's turn: (S) for Snake, (W) for Water, and (G) for Gun: ")

a = game(comp, player)
print(f"Computer choose: {comp}")
print(f"You chose: {player}")
if a == None:
    print("The game is a tie!")
if a == True:
     print("You Win!")
if a == False:
     print("You Lose!")




