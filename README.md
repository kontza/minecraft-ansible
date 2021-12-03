# Introduction
This is the way I roll Minecraft servers.

# Installing
1. Obtain a server JAR, and place it in the repo root.
2. Update `group_vars/all` so that the `server_jar` property matches the name of the server JAR's name.
3. Make sure that both `server_port`, and `world_name` match the values you want.
4. Run `./run-tasks`.
5. Restart `minecraft-***` services.
6. Make sure that they restarted. While upgrading from Spigot 1.17 to Paper 1.17.1, `systemctl restart` didn't restart. I had to `tmux attach` to both servers and `stop` them manually.
