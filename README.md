# Python_Practise
# Number Guess Game

import random

trygame=''

while trygame == '':
    try:
        trygame=int(input("number of game you want to play"))
    except:
        print("please select valid number to play")
for trygame in range (0,trygame):
    choose_no=random.randint(1,26)
    guess=None
    attempt_no=0
    while choose_no != guess:
        try:
            guess=int(input("choose number "))
        except:
            print("please select number to play")
            continue
        if guess != choose_no:
            attempt_no += 1
            if guess>choose_no:
                print("selected no.  higher than matching no.")
            else:
                print("selected no.  lower than matching no.")
        else:
            print("Correct!!!...Number of attempt you took is:: " attempt_no)


