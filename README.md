amahi-install-version-check
===========================

The current Amahi install script doesn't check which version of Ubuntu it is trying to install on.

This version of the script basically checks the /etc/issue for 12041 and lets the user know if Ubuntu 12.04 is detected.

This script will exit if 1210 is detected and let the user know that Amahi only supports 12.04.

[EDIT] Two things to note:

1) The Amahi install script has been updated to provide the same function using a different method.

  -This method checks for the uses sed to remove all letters from `cat /etc/issue` and leave only the numbers associated with the version.
  
  -The current Amahi version removes any text that isn't `Ubuntu LTS` and checks for that string.
  
2) There is a [bash version](https://github.com/aljachimiak/version-check). However, it cannot be used in production because the Amahi version is a Dash script.
