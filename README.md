# password_generator.py

import random
import string

def generate_password(length=12):
    characters = string.ascii_letters + string.digits + "!@#$%^&*"
    return "".join(random.choice(characters) for _ in range(length))

if __name__ == "__main__":
    length = int(input("Password length: "))
    print("Generaed Password:", generate_password(length))
