# Minecraft-Scripts
a few of script the help running a server 

Add these script to the Minecraft Server folder the one with the .JAR make sure to change the version number in Screen.sh to the current version 

now setup the Sytem CTL to start the server on boot so you dont have to use the start.sh file

Step 1
`sudo nano /usr/lib/systemd/system/MinecraftServer.service` #Makes the Service File

Step 2
`sudo nano /etc/systemd/system/MinecraftServer.service` #Edit the service

Step 3
`[Unit]
Description = what service is for
After = network.target

[Service]
Path/Screen.sh` #Edit this Path to the Screen.sh 

`[Install]
WantedBy = multi-user.target`
