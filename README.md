### Overview
Pings is a lightweight and easy-to-use plugin that enhances player communication by automatically tagging players in chat when their name is mentioned. It replaces their name with a custom, styled tag and plays a configurable sound to grab their attention. Perfect for survival servers, PvP servers, or any other environment where fast communication is key!

### Features
- **Customizable Name Tagging**: When a player's name is mentioned in chat, it gets replaced with a custom, configurable text.
- **Sound Alerts**: Plays a sound to the mentioned player so they don’t miss important messages!
- **Fully Configurable**: Change the sound, text style, volume, and pitch directly from the configuration file.
- **Simple Command**: Reload the config easily with `/pings reload`.
- **Permission Support**: Limit who can reload the configuration with permission nodes.

### Commands
- `/pings reload`: Reload the configuration without restarting the server.
  - **Permission**: `nametagger.reload`

### Permissions
- **`nametagger.reload`**: Allows players to reload the configuration with the `/pings reload` command.

### Configuration
Here’s what the default `config.yml` looks like:

```yaml
# The text that replaces the player's name in chat. Use %player% to insert the player's name dynamically.
replacement-text: "&6&l@&f&l%player% &f"

# The sound that plays when a player's name is mentioned in the chat.
# You can choose any valid Minecraft sound from: https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Sound.html
sound: "BLOCK_NOTE_BLOCK_BELL"

# The volume of the sound (1.0 is the maximum).
volume: 1.0

# The pitch of the sound (1.0 is normal, lower values make the sound deeper).
pitch: 0.8
```

### How to Install
1. Download the plugin JAR.
2. Place it into your server’s `plugins` folder.
3. Start the server to generate the config file.
4. Edit the `config.yml` as needed and reload the plugin with `/pings reload`.

### Compatibility
- **Minecraft Versions**: Tested on 1.21, but should work on any modern Bukkit/Spigot version.
- **Dependencies**: None! This plugin is completely standalone.
