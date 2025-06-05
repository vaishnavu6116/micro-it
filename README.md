# micro-it
import random

choices = ["Rock", "Paper", "Scissors"]

def play_round():
    print("Choose: 0 for Rock, 1 for Paper, 2 for Scissors")
    player = int(input("Your choice: "))
    computer = random.randint(0, 2)
    print(f"You chose {choices[player]}, Computer chose {choices[computer]}")

    if player == computer:
        print("It's a draw!")
    elif (player == 0 and computer == 2) or (player == 1 and computer == 0) or (player == 2 and computer == 1):
        print("You win!")
    else:
        print("Computer wins!")

play_round()
