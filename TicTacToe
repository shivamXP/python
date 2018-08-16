state = True
player1 = ''
player2 = ''
currplayer = player1
mylist=['-', '-', '-', '-', '-', '-', '-', '-', '-', '-']
while not player1:
    player1 = input("enter x or o  for player 1: ")

if player1 == 'x':
    player2 = 'o'
else:
    player2 = 'x'

print(player1, player2)


def board(inlist):
    print('{} | {} | {}'.format(inlist[7], inlist[8], inlist[9]))
    print('{} | {} | {}'.format(inlist[4], inlist[5], inlist[6]))
    print('{} | {} | {}'.format(inlist[1], inlist[2], inlist[3]))


def printboard(num, player):
    if player == player1:
        mylist[num] = player1
    else:
        mylist[num] = player2

    board(mylist)


def play1():
    global currplayer
    print(currplayer)
    num = int(input('please enter number : '))
    printboard(num, currplayer)
    checkwin()
    if currplayer == player1:
        currplayer = player2
    else:
        currplayer = player1
    print(''*1000)


def checkwin():
    global state
    if mylist[1] == mylist[2] == mylist[3] and mylist[1] != '-'\
            or mylist[4] == mylist[5] == mylist[6] and mylist[4] != '-' \
            or mylist[7] == mylist[8] == mylist[9] and mylist[7] != '-' \
            or mylist[7] == mylist[5] == mylist[3] and mylist[1] != '-' \
            or mylist[1] == mylist[5] == mylist[9] and mylist[1] != '-' \
            or mylist[7] == mylist[4] == mylist[1] and mylist[1] != '-' \
            or mylist[8] == mylist[5] == mylist[2] and mylist[2] != '-' \
            or mylist[9] == mylist[6] == mylist[3] and mylist[3] != '-':

        print('')
        print(currplayer)
        print('WIN')
        exit(0)


while True:
    play1()










