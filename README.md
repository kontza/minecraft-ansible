# Introduction
This is the way I roll Minecraft servers.

# Installing
1. Run `minecraft_builder group_vars/all`.
2. Use its 'Fetch latest...' functionality to download the latest PaperMC.
3. Update each server's JAR to the one you just downloaded.
4. Run `./run-tasks`.
5. Restart `minecraft-***` services.
6. Make sure that they restarted. While upgrading from Spigot 1.17 to Paper 1.17.1, `systemctl restart` didn't restart. I had to `tmux attach` to both servers and `stop` them manually.
