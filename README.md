# keepercommander-usage
Example usage of [keepercommander](https://pypi.org/project/keepercommander/) by importing it to a python script.

Since I could not find any documentation for using keepcommander library for automation in python script. I have written a sample which can be used to rotate the password in any Website (using selenium) by using Random password generation of keepercommander and save the new generated password back in Keeper Security Vault.

## rotate_passwords.py
This script performs below actions
1. Get the list of Keeper Security Record's UIDs from an Excel file
2. Login to Keeper Security using keepercommander and get the Record Details
3. Goes to Website Address of the record -> Login using its username password -> then to Reset password page
4. Generate a new random password and change in Website
5. Update the new password back to Keeper Security Record

Selenium part for Web navigation is commented as `TODO` as these steps are unique to each site.


