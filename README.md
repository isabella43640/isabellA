# import random
import string

def generate_password(length):
    characters = string.ascii_letters + string.digits + string.punctuation
    password = ''.join(random.choice(characters) for i in range(length))
    return password

print("Welcome to the random password generator!")
length = int(input("How long do you want your password to be? "))
password = generate_password(length)
print("Your random password is:", password)
