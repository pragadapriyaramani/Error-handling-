# Error-handling-
try:
    username = input("Username: ")
    password = input("Password: ")

    if not username or not password:
        raise ValueError("Fields cannot be empty.")

    if username == "admin" and password == "python123":
        print("Login successful!")
    else:
        print("Invalid credentials.")
except ValueError as ve:
    print("Error:", ve)
