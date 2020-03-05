from random import randint

def player_move():
  while True:
    player = str(input(f'{player_name}, choose Rock, Paper, Scissors (R/P/S) or quit Q: ').upper())
    try:
      if player == 'R':
        p_move = move[0]
      elif player == 'P':
        p_move = move[1]
      elif player == 'S':
        p_move = move[2]
      elif player == 'Q':
        quit()
      print(f'{player_name} chooses {p_move}')
      break
    except NameError:
      print('Enter valid choice')
      continue
  return p_move

def computer_move():
  c_move = move[randint(0, 2)]
  print(f'{computer_name} chooses {c_move}')
  return c_move

def win_con(player1_name, player1, player2_name, player2):
  if player1 == 'Rock' and player2 == 'Scissors'or player1 == 'Scissors' and player2 == 'Paper' or player1 == 'Paper' and player2 == 'Rock':
    print(f'{player1_name} is winner, {player1} beats {player2}')
  elif player1 == player2:
    print('It`s a draw')
  else:
    print(f'{player2_name} is winner, {player2} beats {player1}')

if __name__ == '__main__':
  
  player_name = input('Enter name: ')
  computer_name = 'The Computer'
  move = ['Rock', 'Paper', 'Scissors']
  while True:  
    win_con(player_name, player_move(), computer_name, computer_move())
