# Guess-the-number

import random

secret_number = random.randint(1, 10)
guess = None

print("🎯 Guess the number between 1 and 10")

while guess != secret_number:   # != not equal to
    guess = int(input("Enter your guess: "))

    if guess > secret_number:
        print("Too high 🔺")
    elif guess < secret_number:
        print("Too low 🔻")
    else:
        print("🎉 Congratulations! You guessed the number!")
