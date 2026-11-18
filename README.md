# Ambulance Management System

A C console program for managing ambulance records and emergency dispatches.

## Features

- Admin login
- First-run admin account setup with hidden password entry
- A three-attempt limit and five-minute login lockout
- Separate user account registration and login
- User ambulance requests with status tracking
- Admin review and dispatch of user requests
- Add, view, search, update, and delete ambulance records
- Dispatch an available ambulance to an emergency location
- Save ambulance records and dispatch history to text files
- Record the date and time of each dispatch

## Build and run

Open the project folder in VS Code. In the terminal, run:

```bash
clang main.c -o ambulance
./ambulance
```

On first run, choose the admin portal and create an admin username and password. The username must contain letters and numbers. The password must include uppercase and lowercase letters, a number, and a special character, with a maximum of 8 characters. The credentials are saved in `admin_credentials.txt` for future logins.

Choose the user portal to log in or create a user account. Users can submit ambulance requests and view their request status. Admins can review pending requests from menu option 9 and dispatch them when an ambulance is available.

After three failed login attempts, the program locks login for five minutes before allowing another attempt.
