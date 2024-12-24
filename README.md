import secrets
import string

def generate_token(length=32):
    characters = string.ascii_letters + string.digits + string.punctuation
    token = ''.join(secrets.choice(characters) for _ in range(length))
    return token

token = generate_token(32)
print(token)
