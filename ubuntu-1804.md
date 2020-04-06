*After dual boot setup, Ubuntu installed*
Uninstall Amazon and other unnecessary apps, like gaming, from the Ubuntu Software Center.
Remove Thunderbird Mail, Rhythmbox, Help, LibreOffice Writer, Ubuntu Software Center, and Firefox from Favorites in the sidebar Dock.
Run sudo apt update && sudo apt upgrade

Settings Configuration — Open Settings app first
Dock — Switch on “Auto-hide the Dock”. (Reason: I like having more pixels available on my screen to code. Dock takes up unnecessary space.)
Power — Switch off “Automatic Suspend”. (Reason: I don’t want any scripts I might be running to stop because my laptop decided to suspend itself automatically.)
Devices > Mouse & Touchpad — Switch off “Tap to Click”. (Reason: The last thing I want is to keep clicking on the screen by mistake because my hand touches the touchpad while typing.)

*Wifi kept dropping, so took advice to set powersave management to 2 (from 3)
`/etc/NetworkManager/conf.d/default-wifi-powersave-on.conf`
`wifi.powersave = 2`
