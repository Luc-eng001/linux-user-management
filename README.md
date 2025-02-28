##  User account creation script in Linux
Below is a script that automates user creation in Linux

### Script:
#!/bin/bash

# This script creates a new user on the local system.
# Enforces that it be executed with superuser (root) privileges.
# Displays the username, password and host where the account was created.

# Enforces the script to be executed with superuser privileges.
if [[ "${UID}" -ne 0 ]]
then 
	echo 'Run the script with sudo or as root'
	exit 1
fi

# Get the username.
read -p 'Enter the username to create : ' USER_NAME

# Get the real name.
read -p 'Enter the real name of the person who will be using this account : ' COMMENT

# Get the password.
read -p 'Enter the password to use for the new account : ' PASSWORD

# Create the new user.
useradd -c "${COMMENT}" -m ${USER_NAME} 

# Inform the user if the account has been created or not 
if [[ "${?}" -ne 0 ]]
then
	echo 'The account has not been created'
	exit 1
fi

For the full script, check [linux-user-management](creating-local-users.sh)
