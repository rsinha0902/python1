# python1
//For my python codes
//Just to add the codes for all my python exercises

import random
Game = ["Rock", "Paper", "Scissor"]
a = random.choice(Game)
Computer = 0
User = 0
Try = 'Y'
print("You are playing a Game of Rock / Paper / Scissor against Computer")
while Try == "Y":
    print("Enter your option")
    b = str(input())
    if (a==b):
        print("Try Again, you both selected: ",a)
    elif (a=="Rock" and b=="Paper"):
        User = User + 1
        print("Computer Selected: ", a)
        print("Winner User")
    elif(a=="Rock" and b=="Scissor"):
        Computer = Computer + 1
        print("Computer Selected: ", a)
        print("Winner Computer")
    elif(a=="Paper" and b=="Scissor"):
        User = User + 1
        print("Computer Selected: ", a)
        print("Winner User")
    elif (a=="Paper" and b=="Rock"):
        Computer = Computer + 1
        print("Computer Selected: ", a)
        print("Winner Computer")
    elif(a=="Scissor" and b=="Rock"):
        User = User + 1
        print("Computer Selected: ", a)
        print("Winner User")
    elif(a=="Scissor" and b=="Paper"):
        Computer = Computer + 1
        print("Computer Selected: ", a)
        print("Winner Computer")
    print("Do you want to Play again (Y / N)")
    Try = str(input())
if (Computer>User):
    print("Overall Winner is Computer with scores of: ", Computer, " Vs ", User)
else:
    print("Overall Winner is User with scores of: ", User, " Vs ", Computer)
