import random  as m
def game():
    list = ["paper" , "rock" , "scissors" ]
    P = list[:1]   
    R = list[1:2]  
    S = list[2:]   
    computer = m.choice(list)
    player = None
    while player not in list:
        print("Choose one of the following options: ", list)
        player = input()
    if (player == P and computer == R ) or (player == R  and computer == S ) or (player == S  and computer == P ) :
        print("you win! u chooses ", player , "computer chooses " , computer)
    elif player == computer :
        print("Draw, both of you used " , player)
    else : 
        print("you loose ! :( u chooses ", player , "computer chooses " , computer)
list = ["Paper" , "Rock" , "Scissors" ]
y  = ["yes" , "no"]
r = None 
while r not in y :
    print('dou you want to replay:  ' ,  list)
    r = input()
if r == "yes" :
    game()
else : 
    print("then why are u here??")


