# RagnamodVI_Docker W.I.P
Install and maintenance instruction for installing this minecraft forge modpack

## Client installation 
Download the Client manager at https://multimc.org/

- Login into your Mojang account
- Check for the java memory in the client setting
- Check if the clients version by editing the instance of the mods is the same as the server
- PUT DARK mode
- 

## Server installation 
Ragnamod VI 6.0.24 Beta (https://www.curseforge.com/minecraft/modpacks/ragnamod-vi/files/3516953)
https://github.com/Yoosk/ServerStarter
```
mkdir RagnamodVI6.0.24
sudo apt-get install wget unzip
wget https://media.forgecdn.net/files/3516/954/RagnamodVI-Serverfiles-6.0.24.zip
unzip Ragnamod-VI-Beta+6.0.24.zip

vim startserver.sh
# change the mount size
sudo mount -t tmpfs -o size=8G tmpfs "$SAVE_DIR"
# change the maximum ram use
vim server-setup-config.yaml
# specifies the max a mount of ram the server is supposed to launchwith
maxRam: 8G
sudo chmod 666 startserver.sh 
```
