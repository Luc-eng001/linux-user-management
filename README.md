## Linux User Management Scripts

📌 Overview

This repository contains Bash scripts for managing users on a Linux system. These scripts help automate the process of adding and deleting users efficiently, making them useful for system administrators and security professionals.

🚀 Scripts Included

1️⃣ create-linux-user.sh

## Adds a new user to the system.

## Prompts for a username and password.

## Assigns the user to a specific group.

## Enforces a password change on first login.

2️⃣ delete-linux-user.sh

## Deletes an existing user from the system.

## Removes or retains the user's home directory based on the provided option.

## Disables user accounts instead of deleting them (optional).

🛠️ Installation & Usage

Clone the repository to your Linux system:

git clone https://github.com/Luc-eng001/linux-user-management.git

Navigate to the script directory:

cd linux-user-management

Give execution permission to the scripts:

chmod +x create-linux-user.sh delete-linux-user.sh

## Adding a New User

sudo ./create-linux-user.sh

## Deleting an Existing User

sudo ./delete-linux-user.sh

⚠️ Disclaimer

These scripts modify system user accounts. Use with caution, especially in production environments.

🤝 Contributing

Contributions are welcome! To contribute:

## Fork this repository

## Create a new branch (feature-branch)

## Make your changes and commit (git commit -m 'Added feature')

## Push to GitHub and create a Pull Request

📜 License

This project is licensed under the MIT License – see the LICENSE file for details.

⭐ If you find these scripts useful, give this repository a star on GitHub! ⭐
