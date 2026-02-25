# random library
import random

# varible roll the dice to output a random integer from 2 to 12
roll = random.randint(2, 12 )

# Input and asking the user to guess the dice number that will be rolled
# try is used for a safe measure for error and will be escaped on except value
try:
    guess = int(input('Guess the dice roll numbers from 2 to 12: '))
    # 
    if guess == roll:
        print(f"Correct! The dice rolled a {roll}")
    else:
        print(f"Close! The dice actually rolled a {roll}. Better luck next time!")
#safe measure if the user spells the number
except ValueError:
    print("Oops! Please enter a number, not text.")
