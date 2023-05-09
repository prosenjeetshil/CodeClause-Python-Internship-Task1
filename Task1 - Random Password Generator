import string
import random

# user input for password length
while True:
    try:
        length = int(input("Enter the password length you wish for: "))
        break
    except ValueError:
        print("Invalid input. Please enter a numeric value.")


# character choices according to user
character_list = ""

print('''Choose the character set for password from these:
        1. Digits
        2. Letters
        3. Special characters
        4. Exit''')

while True:
    choice = int(input("Pick a number: "))
    if choice == 1:
        character_list += string.digits
    elif choice == 2:
        character_list += string.ascii_letters
    elif choice == 3:
        character_list += string.punctuation
    elif choice == 4:
        break
    else:
        print("Please pick a valid option!")

password = []
for i in range(length):
    randomchar = random.choice(character_list)
    password.append(randomchar)

# Print the password as a string
print("The random password is " + "".join(password))
