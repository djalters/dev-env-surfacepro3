*After dual boot setup, Ubuntu installed*
Uninstall Amazon and other unnecessary apps, like gaming, from the Ubuntu Software Center.
Remove Thunderbird Mail, Rhythmbox, Help, LibreOffice Writer, Ubuntu Software Center, and Firefox from Favorites in the sidebar Dock.
Run sudo apt update && sudo apt upgrade

Put the following lines in your ~/.inputrc:
```
## arrow up
"\e[A":history-search-backward
## arrow down
"\e[B":history-search-forward
```

Settings Configuration — Open Settings app first
Dock — Switch on “Auto-hide the Dock”. (Reason: I like having more pixels available on my screen to code. Dock takes up unnecessary space.)
Power — Switch off “Automatic Suspend”. (Reason: I don’t want any scripts I might be running to stop because my laptop decided to suspend itself automatically.)
Devices > Mouse & Touchpad — Switch off “Tap to Click”. (Reason: The last thing I want is to keep clicking on the screen by mistake because my hand touches the touchpad while typing.)

*Wifi kept dropping, so took advice to set powersave management to 2 (from 3)
`/etc/NetworkManager/conf.d/default-wifi-powersave-on.conf`
`wifi.powersave = 2`

Create ssh key
`ssh-keygen -t rsa -b 4096 -C "walters.eye@gmail.com"`
to run, start in background
```
$ eval "$(ssh-agent -s)"
> Agent pid 59566
```
add key to agent
`ssh-add ~/.ssh/id_rsa`

Python3
- should already be installed with ubuntu
-install pip3-pyth
