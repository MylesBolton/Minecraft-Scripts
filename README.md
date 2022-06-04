# Minecraft-Scripts
a few of script the help running a server 

Add these script to the Minecraft Server folder the one with the .JAR make sure to change the version number in Screen.sh to the current version 

now setup the Sytem CTL to start the server on boot so you dont have to use the start.sh file

Step 1 - Edit the Service File
`sudo nano /etc/systemd/system/MinecraftServer.service`

Step 2 - copy the contets of the `MinecraftServer.service` File in the repo and paste it into the file you are editing Make sure you edit the Path for the Service to the Screen.sh file

Step 3 - Enable the Service
`sudo systemctl enable MinecraftServer.service`

Step 4 - Start the Service 
`sudo systemctl start MinecraftServer.service`

Step 5 - Check the Status of the Service 
`sudo systemctl status MinecraftServer.service`
