## π Paper server
Already configured Minecraft server based on [@PaperMC](https://github.com/PaperMC) core to use on low-end hardware for Linux-based OS

### π€ What files are configured?
1. server.properties β Minecraft server config
2. bukkit.yml β CraftBukkit config
3. spigot.yml β Spigot core config (since Spigot is a fork of CraftBukkit)
4. paper.yml β Paper core config (since Paper is a fork of Spigot)
4. start.sh β bash script to start the server (mostly took from [@Dymeth](https://github.com/Dymeth))

### π How to run the server?
Please type `sh ./start.sh` in terminal
or:
```
chmod 700 start.sh
./start.sh
```
(to run the script as executable)

### π‘ Features of the startup bash script
1. Restarts the server on its crash or stop (to stop completely βΒ press Ctrl+C on restart countdown)
2. Includes [@aikar](https://github.com/aikar)'s JVM optimization flags
3. Runs the server in a new screen (server won't stop if you corrupt the SSH session)
4. Easy-to-configure JVM basic flags as the maximum RAM usage
5. Preconfigured JVM flags as nogui flag that's useless in CLI
