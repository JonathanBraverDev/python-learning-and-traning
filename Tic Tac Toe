EMPTY_BOARD = (
    ['-', '-', '-'],
    ['-', '-', '-'],
    ['-', '-', '-']
)

# returns a set (order doesn't matter here) of all free spaces on the board
def free_spots(board):

    result = set()
    for i in range(len(board)):
        for j in range(len(board[i])):
            if board[i][j] == '-':
                result.update([(j, i)])
    return result


# adds the player's 'marker' (currently only X) to the given location
def move(board, x, y):
    board[y][x] = 'X'


loop = True
game_board = EMPTY_BOARD

while loop:

    print(game_board)
    print(free_spots(game_board))
    inputY = int(input('enter the row of your move '))
    inputX = int(input('enter the tile of your move '))
    destination = (inputX, inputY) # (definitely looks better than cramming all of this to the same line)

    # looks for the inputted position in the set of available moves
    if destination in free_spots(game_board):
        move(game_board, inputX, inputY)
        print(game_board)
    else:
        print('the tile is taken, please try again')
        
    # to stop a bad behaving game
    ans = input('keep playing? (n to stop)')
    if ans == 'n':
        loop = False
