# Rock-Paper-and-Scissor-Project-using-Python
I have started learning python and I have made a basic project using python i.e, Rock, Paper and Scissor
I have used Nested IF-ELSE statement
Firstly I imported a python library, random using import random.
random function gives random numbers between selected starting and ending numbers

I have taken 3 variables rock, paper and scissor and assigned strikers for those three variables.
Created a list of three variables with a variable name, 'game_images'.
0 - Rock
1 - Paper
2 - Scissor

There should be user input and computer input. Depending upon the two inputs we decide who is winner. 
user input will be taken using input function.
Computer input will be taken using random.randint function

If a user enter a number other than 0, 1, 2. It will print as "Enter a number between 0 1 2.
In ELSE part I used nested if to give all conditions of the game.
If user input is equal to 0 and computer is equal to 2
it print as 'You win'

If user input is equal to 2 and computer is equal to 0
it print as 'You loss'.

if user choice is greater than computer choice
'You win'

if computer choice is greater than user choice
'You loss'

if both inputs are equal,
it print as 'Draw'

user_choice > 2 or user_choice <0) and (computer_choice >2 or computer_choice < 0
it print as 'You have entered wrong input'

If any of the coditions are not satisfies, in else part we print as 'You have entered wrong input'.

    import random 
    rock = '✊'
    paper = '✋'
    scissor = '✌️'
    
    # Values are taken for above 3 variables as stricker images from the internet
    
    game_images = [rock, paper, scissor] # Created a list of three variables
    user_choice = int(input("0 for Rock, 1 for Paper, 2 for Scissor: "))  #User iput is taken using input function
    
    # By default input function is in string format. so we are using int function to covert string to integer
    
    if user_choice >= 3 or user_choice < 0:
        print("Enter numbers between 0 to 1")
    
    else:
    print(game_images[user_choice])
    computer_choice = random.randint(0, 2)
    print(f"Computer choice: {computer_choice}")
    print(game_images[user_choice])
    
    if user_choice == 0 and computer_choice == 2:
        print("You Win")
    
    elif user_choice == 2 and computer_choice == 0:
        print("You Loss")
    
    elif user_choice > computer_choice:
        print("You Win")
    
    elif computer_choice > user_choice:
        print("You Loss")
    
    elif user_choice == computer_choice:
        print("Draw")
    
    elif (user_choice > 2 or user_choice <0) and (computer_choice >2 or computer_choice < 0):
        print("You have entered wrong input")
    
    else:
        print("You have entered wrong input")


 

