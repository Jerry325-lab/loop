# loop
player_position = 3
score = 0
speed = 1.0
streak = 0
game_running = True
while game_running:
    rock_position = random.randint(1, 5)
    print(f"Rock is falling in lane {rock_position}")
    print("player score is 0")

    move = input("Move (L/R/Q): ").strip().upper()

    if move == "Q":
        print("You quit the game!")
        break

if move == "L":
    rock_position = random.randint(1, 1)

if move == "R":
    rock_position = random.randint(1, 5)

else: print("You stayed in the same lane.")


if player_position == rock_position:
    print("Hit and Break")

else:
    print("You dodged the rock.")
    score += 10
    streak += 1

print(f"The rock are falling faster!")

if streak == 3:
    print("DODGE STREAK!")
if streak == 2:
    print("RESET STREAK")


print(f"[1][2][3][4][5]")
print(f"rock in {rock_position} / player {player_position}")

print(f"Game Over! Your final score was {score}")
print("Thanks for playing DODGE THE ROCKS!")


print("Welcome to DODGE THE ROCKS!")
print("Avoid the falling rocks as long as you can!")
print("Use 'L' to move left, 'R' to move right, and 'Q' to quit.\n")
