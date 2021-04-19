import random
# use code below  to generate a random integer between 30 and 50 for example
#print(random.randint(30, 50))

# ********************************** YOUR CODE GOES BELOW HERE *********************************************************
secret = random.randint(30, 50)
print('I am thinking of a number between 1 and 99')
guess = int(input("Enter a guess: "))
while secret != guess:
    if guess < secret:
        print("Your guess is too low. Try again!")
        guess = int(input("Enter a guess: "))
    else:
        print("Your guess is too high, Try again!")
        guess = int(input("Enter a guess: "))

print("Congrats! You guessed right!")
