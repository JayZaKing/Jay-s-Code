import random
user_input= str(input("Choose rock, paper or scissors"))
computer_input = random.randint(1,3)
if computer_input == 1:
    print("The computer has chosen rock")
elif computer_input == 2:
    print("The computer has chosen paper")
elif computer_input ==3:
    print("The computer has chosen scissors")
else:
    quit()

if user_input == "rock":
    print("You have chosen rock")
elif user_input == "paper":
    print("You have chose paper")
elif user_input == "scissors":
    print("You have chose scissors")
else:
    quit()
def winner_or_loser(user_input,computer_input):
    
    print(user_input, computer_input)
    if user_input == computer_input:
        print("Tie")
    elif user_input == "rock" and computer_input == "paper":
        print("The computer has won")
    elif user_input == "paper" and computer_input == "rock":
        print("You have won!")
    elif user_input == "scissors" and computer_input == "paper":
        print("You have won")
    elif user_input == "paper" and computer_input == "scissors":
        print("The computer has won")
    elif user_input == "rock" and computer_input == "scissors":
        print("You have won")
    elif user_input == "scissors" and computer_input == "rock":
        print("The computer has won")

winner_or_loser(user_input, computer_input)
