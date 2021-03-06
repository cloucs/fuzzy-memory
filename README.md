# fuzzy-memory
Beginner cheat sheet for the Arch Linux terminal

## Terminology
Symbol | Description
---|---
~/ | Home directory
."file name" | dot files / hidden files
| | Pipe operator

## General
Shortcut | Description
---|---
sudo "program name" | Run program as super user
sudo !! | Runs last used command as sudo
history | Lists all used commands
cd "path" | Change directory to specified path
cd .. | Change directory to parent directory
cd | Change directory to home directory
ls "path" | Lists files in specified directory
ls | Lists files in current directory
mkdir "directory name" | Create directory

## Pacman (Package Manager)
Shortcut | Description 
---|---
sudo pacman -Syy | Update package lists 
sudo pacman -Syu | Full system upgrade
sudo pacman -S "package name" | Install package
sudo pacman -Rs "package name" | Remove package and unneeded dependencies

## Nano (Text editor)
Shortcut | Description 
---|---
nano | Start nano
Ctrl+o | Save file
Ctrl+x | Exit file

### Set nano as default editor
`$ echo "export EDITOR=/usr/bin/nano" >> ~/.zshrc`

`$ echo "export VISUAL=/usr/bin/nano" >> ~/.zshrc`

## Systemd (System and service manager)
Shortcut | Description
---|---
sudo systemctl start "daemon name" | Start daemon / service
sudo systemctl stop "daemon name" | Stop daemon / service
sudo systemctl enable "daemon name" | Enable Autostart daemon / service
sudo systemctl disable "daemon name" | Disable Autostart daemon / service
sudo systemctl status "daemon name" | Status of daemon / service
