# TOTPPowerShellModule
Module for TOTP Client for PowerShell

I created a module for easier user. I did not create the OTP code.

Source: https://gist.github.com/jonfriesen/234c7471c3e3199f97d5

# How to use
```posh
# otp is alias for Get-OTP

# Generate OTP code with 30 seconds window, 6 digit length:
> otp secretkeystring
856181

# Generate OTP code with 20 seconds window, 8 digit length:
> otp secretkeystring -WINDOW 20 -LENGTH 8
72406208

# With all parameters specified, not using alias
> Get-Otp -SECRET 'secretkeystring' -WINDOW 22 -LENGTH 5
18017
```
