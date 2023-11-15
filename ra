import time

def introduction():
    print("Welcome to the Adventure Game!")
    print("You find yourself standing at the entrance of a mysterious cave.")
    print("Your goal is to explore the cave and make decisions that will lead to different outcomes.")
    print("Let the adventure begin!\n")

def make_choice(choices):
    while True:
        print("Choose your action:")
        for i, choice in enumerate(choices, 1):
            print(f"{i}. {choice}")

        try:
            choice_num = int(input("Enter the number of your choice: "))
            if 1 <= choice_num <= len(choices):
                return choice_num
            else:
                print("Invalid choice. Please enter a valid number.")
        except ValueError:
            print("Invalid input. Please enter a number.")

def explore_cave():
    print("\nYou enter the cave and see two tunnels.")
    time.sleep(1)
    print("To the left, you hear a mysterious sound.")
    print("To the right, you see a faint light.")
    choices = ["Go left", "Go right"]
    choice = make_choice(choices)

    if choice == 1:
        left_tunnel()
    elif choice == 2:
        right_tunnel()

def left_tunnel():
    print("\nYou decide to go left.")
    time.sleep(1)
    print("As you venture deeper, the mysterious sound becomes louder.")
    print("You encounter a friendly creature playing music.")
    choices = ["Join the creature in a dance", "Continue exploring"]
    choice = make_choice(choices)

    if choice == 1:
        print("\nThe creature is delighted! You spend a joyful time dancing together.")
        print("Congratulations! You've found a friend in the cave. Game Over.")
    elif choice == 2:
        print("\nYou decide to explore further. The sound fades, and you discover a hidden treasure.")
        print("Congratulations! You've found a treasure in the cave. Game Over.")

def right_tunnel():
    print("\nYou choose to go right.")
    time.sleep(1)
    print("The faint light leads you to an underground garden with glowing plants.")
    print("You see a path going up and a path going down.")
    choices = ["Go up", "Go down"]
    choice = make_choice(choices)

    if choice == 1:
        print("\nYou ascend the path and find an exit. Congratulations! You've successfully left the cave. Game Over.")
    elif choice == 2:
        print("\nYou descend into the depths of the cave and discover a secret chamber.")
        print("Inside the chamber, you find ancient knowledge.")
        print("Congratulations! You've gained wisdom from the cave. Game Over.")

def main():
    introduction()
    explore_cave()

if __name__ == "__main__":
    main()
