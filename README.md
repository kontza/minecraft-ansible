# Introduction
This is the way I roll Minecraft servers.

# Installing
1. Obtain a server JAR from https://papermc.io/downloads, and place it in the repo root.
2. Run `minecraft_builder group_vars/all` and update each server's JAR to the one you just downloaded.
3. Run `./run-tasks`.
4. Restart `minecraft-***` services.
5. Make sure that they restarted. While upgrading from Spigot 1.17 to Paper 1.17.1, `systemctl restart` didn't restart. I had to `tmux attach` to both servers and `stop` them manually.
