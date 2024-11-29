# Treasure-Island

This project is a text-based adventure game called "Treasure Island," implemented in Python. The game takes the player on an exciting journey to find hidden treasure on a mysterious island. Players make choices at each step, leading them through different paths and outcomes.

## Features

- **Interactive Gameplay**: Players make choices that affect the outcome of the game.
- **Multiple Endings**: Different choices lead to various endings, adding replay value.
- **Text-Based Adventure**: Engaging narrative and descriptions to immerse players in the adventure.

## Technologies Used

- **Python**: The programming language used to implement the game logic.

## How to Run the Game

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/treasure-island.git
   cd treasure-island
   ```

2. **Run the Game**:
   ```bash
   python treasure_island.py
   ```

## Code Explanation

### Python Code

The Python code implements the game logic, including player choices and different outcomes based on those choices.

```python
print('''
***************************
          |                   |                  |                     |
 ___|_____.="";=._____|_______|__
|                   |  ,-"_,=""     `"=.|                  |
|______|"=._o`"-.        `"=._____|______
          |                "=._o"=._      `"=.                     |
 ___|_______:=.o "=..".-="'"=.______|__
|                   |    _.--" , ; `"=._o." ,-"""-. ".   |
|______|."  ,. .` ` `` ,  `"-."-._   ". '_|______
          |           |o`"=.` , "` `; .". ,  "-."-._; ;              |
 ___|____| ;-.o"=.; ." ` '."\ . "-._ /_____|___
|                   | |o;    "-.o"=.``  '` " ,_.--o;   |
|______|| ;     (#) -.o `"=..--"_o.-; ;_|______
_/__/__/_|o;.    "      `".o|o_.--"    ;o;_/__/__/_
/__/__/__/"=._o--.        ; | ;        ; ;/__/__/__/_
_/__/__/__/"=._o--.   ;o|o;     .;o;_/__/__/_
/__/__/__/__/_"=._o.; | ;.--"o.--"/__/__/__/_
_/__/__/__/__/_"=.o|o.--""_/__/__/__/__
/__/__/__/__/__/__/__/__/__/__/___ /
***************************
''')
print("Welcome to Treasure Island.")
print("Your mission is to find the treasure.") 

#Write your code below this line 👇

choice1 = input('You\'re at a cross road. Where do you want to go? Type "left" or "right" \n').lower()
if choice1 == "left":
  choice2 = input('You\'ve come to a lake. There is an island in the middle of the lake. Type "wait" to wait for a boat. Type "swim" to swim across. \n').lower()
  if choice2 == "wait":
    choice3 = input("You arrive at the island unharmed. There is a house with 3 doors. One red, one yellow and one blue. Which colour do you choose? \n").lower()
    if choice3 == "red":
      print("It's a room full of fire. Game Over🔴.")
    elif choice3 == "yellow":
      print("You found the treasure! You Win!🟡✨")
    elif choice3 == "blue":
      print("You enter a room of beasts. Game Over🔵.")
    else:
      print("You chose a door that doesn't exist. Game Over.")
  else:
    print("You get attacked by an angry trout. Game Over.")
else:
  print("You fell into a hole. Game Over😐.")
  print("thank you for participating , play agin")
```

### Explanation:

1. **Introduction**:
   - The game starts with a welcome message and the player's mission to find the treasure.

2. **Game Map**:
   - The ASCII art represents the treasure map, setting the scene for the adventure.

3. **First Choice**:
   - The player is prompted to choose between "left" or "right" at a crossroad.
   - If the player chooses "left," they proceed to the next choice. If "right," the game ends with "Game Over."

4. **Second Choice**:
   - The player encounters a lake and must choose to "wait" for a boat or "swim" across.
   - If the player chooses "wait," they proceed to the next choice. If "swim," the game ends with "Game Over."

5. **Third Choice**:
   - The player arrives at an island with three doors (red, yellow, blue) and must choose one.
   - Depending on the player's choice, they either find the treasure and win or encounter a fatal scenario and the game ends with "Game Over."

6. **Game Over Messages**:
   - Different endings are provided based on the player's choices, adding variety and replay value to the game.
