# 🌊 Digispark Script - Reverse Shell
- Completed On: February 1th 2023

### How to use:

### DigiSpark Reverse Shell Script:
This DigiSpark script downloads and executes the Invoke-PowerShellTcpOneLine.ps1 powershell script which essentially opens a netcat reverse shell from a Windows machine to the host computer in about 3 seconds.

#### Instructions:
  ### On the host machine (I assume you are using linux for this):
  1. Open a netcat listener on a port (the script uses port 4444 by default): `nc -lp 4444`
  2. Download and modify the Invoke-PowerShellTcpOneLine.ps1 by removing the first line comment and changing the IP address to the one of your host machine and the port to the one you chose earlier.
  3. You now need to host the payload on a web server so it can be downloaded on the Windows computer. There are many ways to do this, but for anyone who wants a quick and easy solution you can host a php web server from the linux terminal like this: `sudo php -S 0.0.0.0:80 -t /directory/to/folder/of/powershellScript/`
  4. Download and edit the `Reverse_Shell.ino` DigiSpark script to match the address where the ps1 powershell script is hosted and compile and load `Reverse_Shell.ino` to your DigiSpark. 
  
  ### On the Windows machine:
  Plug in the DigiSpark and enjoy your reverse shell on the host machine!
  
Hope you all enjoy this script and as always use it responsibly!

## 🐬 Find me here!
- [![social](https://img.shields.io/static/v1?logo=twitter&link=https://twitter.com/m6sser&label=&message=m6sser&color=white&logoColor=white&style=flat&labelColor=4f94ef)](https://twitter.com/m6sser)
[![social1](https://img.shields.io/static/v1?logo=instagram&link=https://instagram.com/fmesser11&label=&message=fmesser11&color=white&logoColor=white&style=flat&labelColor=4f94ef)](https://instagram.com/fmesser11)
[![social2](https://img.shields.io/static/v1?logo=GitHub&link=https://github.com/m6sser&label=&message=m6sser&color=white&logoColor=white&style=flat&labelColor=4f94ef)](https://github.com/m6sser)
[![social3](https://img.shields.io/static/v1?logo=Discord&link=http://discordapp.com/users/974844018762588200&label=&message=m6sser%232396&color=white&logoColor=white&style=flat&labelColor=4f94ef)](http://discordapp.com/users/974844018762588200)
