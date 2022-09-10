# Project One Code (QuizGame)
~~~ python
#Welcome statement
print("Welcome to my QuizGame!")
#Asking to play
playing = input("Do you want to play this game? ")

if playing.lower() != "yes":
    quit()
print("Great! Lets play ")
score = 0
#Asking questions

answer = input("What does CPU stands for? ")
if answer.lower() == "central processing unit":
    print("Correct!")
    score += 1
else:
    print("Ops!, Incorrect!")

answer = input("What does GPU stands for? ")
if answer.lower()  == "graphics processing unit":
    print("Correct!")
    score += 1
else:
    print("Ops!, Incorrect!")

answer = input("What does RAM stands for? ")
if answer.lower()  == "random access memory":
    print("Correct!")
    score += 1
else:
    print("Ops!, Incorrect!")

answer = input("What does PSU stands for? ")
if answer.lower()  == "power supply":
    print("Correct!")
    score += 1
else:
    print("Ops!, Incorrect!")

answer = input("What does ROM stands for?  ")
if answer.lower()  == "read only memory":
    print("Correct!")
    score += 1
else:
    print("Ops!, Incorrect!")

answer = input("What does DS stands for?  ")
if answer.lower()  == "data science":
    print("Correct!")
    score += 1
else:
    print("Ops!, Incorrect!")
#printing correct score
print("You got " + str(score) + " questions correct! ")
print("You got " + str(score/6*100) + " %") 
~~~ 

## Project Two Code (Number Guessing Game)
~~~ python 
import random

top_of_range = input("Type a number: ")
if top_of_range.isdigit():
    top_of_range = int(top_of_range)
    if top_of_range<=0:
        print("Please type a digit greater 0 next time.")
        quit()
else:
    print("please type a number next time")
    quit()
# will generate random numbers
random_number = (random.randrange(0,top_of_range))
guesses =0


while True:
    guesses +=1
    user_guess = input("Make a guess:  ")
    if user_guess.isdigit():
        user_guess = int(user_guess)
    else:
        print("please type a number next time")
        quit()
        continue
    if user_guess == random_number:
        print("You got it correct")
        break
    elif user_guess > random_number:
        print("You guessed greater than the number!")
    elif user_guess < random_number:
        print("You guessed lesser than the number!")

print("You got it in",guesses, "guesses")
~~~
## Project Three code (Rock, Paper, Scissors)
~~~ python
import random

user_wins= 0
computer_wins = 0

options = ["rock","paper","scissors"]

while True:
    user_input = input("Type Rock/Papr/Scissors or Q to quit: ").lower()
    if user_input == "q":
        break
    if user_input not in options:
        continue
    random_no = random.randint(0, 2)
    # rock:0, paper:1, scissors:2
    computer_pick = options[random_no]
    print("computer picked", computer_pick + ".")

    if user_input == "rock" and computer_pick == "scissors":
        print("y0u won!")
        user_wins += 1

    elif user_input == "paper" and computer_pick == "rock":
        print("you won!")
        user_wins += 1

    elif user_input == "scissors" and computer_pick == "paper":
            print("you won!")
            user_wins += 1
    else:
        print("you lost, computer wins")
        computer_wins += 1
print("you won", user_wins, "times")
print("computer won", computer_wins, "times")


print("Goodbye!")
~~~
