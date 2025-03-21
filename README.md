# GrubRestarterWindows

Bored on restarting, waiting for boot and switch manually on grub?
Want to restart on Linux and meanwhile go take a dump?
This is the solution.

## Description
Enables you through a script to restart on any distro you want from Windows


## Usage
Start the script through powershell in admin mode

## Requirements
Written as comments in the script file, I'd like pull requests with improvements, I'm not really into powershell scripting :)

- Be sure to visudo and add your username or group you're in with the permission to use sudo commands with **NO password**
- Find the drive you installed the bootloader in and modify \\.\PHYSICALDRIVE1 on wsl --mount command
- Watch the first time under what name the drive is mounted in WSL with lsblk and edit it if necessary on wsl --exec sudo mount command
- If you don't want to start on the **first option of grub** (index 0) decode base64 and edit the number 0 with the index you prefeer, then paste the base64 back in.
- Enjoy :)
