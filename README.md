# CODSOFT_3
# Task 3 : Password generation
import string
import random

# Generating password with the help of python

# Taking input of the password length from the user
password_length = int(input("Enter the length of the password : "))

# Generating password
letters = string.ascii_letters
digits = string.digits
punctuations = string.punctuation

# Taking combination of letters, digits and punctuations
Characters = letters + digits + punctuations
password = ""
for i in range(password_length):
    # Picking up a random character from the character list
    Random_char= random.choice(Characters)
    # Adding a random character to the empty string i.e passwrod
    password += Random_char

# Displaying a random password to the user
print(password)
