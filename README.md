# Playworks_Coding_Factory
import random
c = ["Rock", "Paper", "Scissors"]


count = 0
compcount = 0
while True:
        b = ['Y', 'N']
        a = input("Play Game? Y/N ")
        if a not in b:
            print("Error: Invalid Character Entry")
        elif a == b[0]: 
            b = input("Choose: Rock, Paper, Scissors ")
            d = random.choice(c)
            if b == "Rock" and d == "Scissors":
                count = count + 1 
                print (d)
                print ("You Win") 
            elif b == "Rock" and d == "Paper":
                compcount = compcount + 1
                print (d)
                print ("You lose")
            elif b == "Rock" and d == "Rock":
                print(d)
                print ("Tie")
            if b == "Scissors" and d == "Scissors":
                print (d)
                print ("Tie")
            elif b == "Scissors" and d == "Paper":
                count = count + 1
                print (d)
                print ("You Win")
            elif b == "Scissors" and d == "Rock":
                compcount = compcount + 1
                print(d)
                print ("You Lose")
            if b == "Paper" and d == "Scissors":
                compcount = compcount + 1
                print (d)
                print ("You Lose")
            elif b == "Paper" and d == "Paper":
                print (d)
                print ("Tie")
            elif b == "Paper" and d == "Rock":
                count = count + 1
                print(d)
                print ("You Win")
        else:
            if a == b[1]:
                print("Game Over")
                break

print ("Score: You", count, "Computer", compcount)
    
    
        
