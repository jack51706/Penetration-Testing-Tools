## Windows penetration testing related scripts, tools and Cheatsheets


- **`awareness.bat`** - Little and quick Windows Situational-Awareness set of commands to execute after gaining initial foothold (coming from APT34: https://www.fireeye.com/blog/threat-research/2016/05/targeted_attacksaga.html ) ([gist](https://gist.github.com/mgeeky/237b48e0bb6546acb53696228ab50794))

- **`Force-PSRemoting.ps1`** - Forcefully enable WinRM / PSRemoting. [gist](https://gist.github.com/mgeeky/313c22def5c86d7a529f41e5b6ff79b8)

- **`GlobalProtectDisable.cpp`** - Global Protect VPN Application patcher allowing the Administrator user to disable VPN without Passcode. ([gist](https://gist.github.com/mgeeky/54ac676226a1a4bd9fd8653e24adc2e9))

    Steps are following:
    
    1. Launch the application as an Administrator
    2. Read instructions carefully and press OK
    3. Right-click on GlobalProtect tray-icon
    4. Select "Disable"
    5. Enter some random meaningless password
    
    After those steps - the GlobalProtect will disable itself cleanly. 
    From now on, the GlobalProtect will remain disabled until you reboot the machine (or     restart the PanGPA.exe process or PanGPS service).

- **`impacket-binaries.sh`** - Simple one-liner that downloads all of the Windows EXE impacket binaries put out in [Impacket Binaries](https://github.com/ropnop/impacket_static_binaries) repo. [gist](https://gist.github.com/mgeeky/2f990f14f1e7cf78fce21b8761234604)

- **`pth-carpet.py`** - Pass-The-Hash Carpet Bombing utility - trying every provided hash against every specified machine. ([gist](https://gist.github.com/mgeeky/3018bf3643f80798bde75c17571a38a9))

- **`revshell.c`** - Utterly simple reverse-shell, ready to be compiled by `mingw-w64` on Kali. No security features attached, completely not OPSEC-safe.

- **`Simulate-DNSTunnel.ps1`** - Performs DNS Tunnelling simulation for purpose of triggering installed Network IPS and IDS systems, generating SIEM offenses and picking up Blue Teams.

- **`win-clean-logs.bat`** - Batch script to hide malware execution from Windows box. Source: Mandiant M-Trends 2017. ([gist](https://gist.github.com/mgeeky/3561be7e697c62f543910851c0a26d00))
