amahi-install-version-check
===========================

The current Amahi install script doesn't check which version of Ubuntu it is trying to install on.

This version of the script basically checks the /etc/issue for 12041 and lets the user know if Ubuntu 12.04 is detected.

This script will exit if 1210 is detected and let the user know that Amahi only supports 12.04.
