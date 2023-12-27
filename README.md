# guess-game-
guessing an integer number 
import random
def guess(x):
    random_number=random.randint(1,x)
    guess=0
    while guess!=random_number:
        guess=int(input(f"enter the guess between 1 and {x}: "))
        if guess<random_number:
            print("too low , guess again")
        elif guess>random_number:
            print("too high, guess again")
    else:
        print("good job ,your guess was right ")
guess(100)
