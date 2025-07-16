Correct local generation login/password on python


import bcrypt

def encrypt_password(username, password):
    bcrypted = bcrypt.hashpw(password.encode("utf-8"), bcrypt.gensalt(prefix=b"2a")).decode("utf-8")
    return f"{username}:{bcrypted}"

print(encrypt_password("login", "password"))