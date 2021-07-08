import random

draw = 0
win=0
loss=0

def valid_move():
  print("enter your move: r for rock, p for paper, s for scissor, q for quit")
  while True:
    player_move=input().lower()
    if player_move in ['r','p','s','q']:
      return player_move
    else:
      print("Wrong Input, Enter again")
      
while True:
  print("\n")
  print("======Rock Scissor Paper======")
  print("\n")
  print('%s Win, %s Loss, %s Draw' % (win, loss, draw))
  print("\n")

  player_move = valid_move()
  computer_random = random.randint(1,3)

  if player_move=="q":
    print("You are quiting ;(")
    break
  elif player_move == "r":
    print("You choose rock")
  elif player_move=="p":
    print("You choose paper")
  elif player_move=="s":
    print("You choose scissor")

  #computer_move
  if computer_random ==1:
    computer_move="r"
    print("Computer chooses rock")
  elif computer_random==2:
    computer_move="p"
    print("Computer chooses paper")
  elif computer_random==3:
    computer_move="s"
    print("Computer chooses scissor")

  # check player_move with computer move

  if player_move== computer_move:
    print("IT'S DRAW")
    draw+=1
  #player wins

  elif player_move=="r" and computer_move=="s":
    print("You win")
    win +=1
  elif player_move=="p" and computer_move=="r":
    print("You win")
    win +=1
  elif player_move=="s" and computer_move=="p":
    print("You win")
    win +=1

  #player lose
  elif player_move == "r" and computer_move=="p":
    print("You lose")
    loss +=1
  elif player_move == "p" and computer_move=="s":
    print("You lose")
    loss+=1
  elif player_move == "s" and computer_move=="r":
    print("You lose")
    loss +=1
