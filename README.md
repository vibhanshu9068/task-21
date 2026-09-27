# task-21
import string
import secrets

# Ask the user for password length
length = int(input("Enter password length: "))

# Characters for password
characters = string.ascii_letters + string.digits + string.punctuation

# Generate random password
password = ''.join(secrets.choice(characters) for _ in range(length))

# Display password
print("Your strong password is:", password)
