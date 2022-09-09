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

# # Project Two Code (Number Guessing Game)
~~~ 

~~~
