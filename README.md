# Harmonica - Discord Music Bot

Presenting " Harmonica " This self hosted bot uses YT-DLP to download audio files from YouTube and Spotify to play them directly in your Discord voice channel.

Currently it is considered Work In Progress, it has and will have bugs, but the general idea is there and works.

![image](https://github.com/user-attachments/assets/e5f51fc2-994c-4e54-9702-650040512182)
![image](https://github.com/user-attachments/assets/1b1d18f3-fd22-44be-8069-f3f4098bddb1)
![image](https://github.com/user-attachments/assets/2a486230-cc0c-476d-8ccf-f65075ff09fe)
![image](https://github.com/user-attachments/assets/f60c7ce9-295b-457c-90c2-81375da8b18c)
![image](https://github.com/user-attachments/assets/4974cabd-10c0-41cf-a996-2562baa9b52e)

## Setup

### Prerequisites
1. **Python**: Ensure you have Python 3.8 or higher installed.
2. **Dependencies**: Install the required Python packages using the following command:
   ```bash
   pip install -r requirements.txt
   ```

### Platform-Specific Instructions
- **Windows**: If `ffmpeg` is installed during the first initialization, you will need to relaunch the `bot.py` script.
- **macOS**: If `ffmpeg` fails to install automatically, manually place `ffmpeg` in the root directory.
- **Linux**: The setup script will automatically handle `ffmpeg` installation.
- **General**: yt-dlp, spot-dl and ffmpeg will be downloaded and set up automatically.

3. **Environment Variables**: Rename the `.env.example` file to `.env` and add your Discord bot token:
   ```
   DISCORD_TOKEN=your_token_here
   ```

4. **Cookies**: Import cookies.txt using the [Get Cookies.txt extension](https://chromewebstore.google.com/detail/get-cookiestxt-locally/cclelndahbckbenkjhflpdbgdldlbecc) and place it in the root directory.

5. **Run the Bot**: Start the bot using the following command:
   ```bash
   python bot.py
   ```

## Features
- **Play Music**: Stream music from YouTube directly into your Discord voice channel.
- **Playback Controls**: Basic controls like play, pause, skip, and stop.
- **Queue System**: Manage a queue of songs to play in sequence.
- **Loop Mode**: Toggle loop mode for continuous playback of the current song.

## Commands
- `!help` - Display this help message.

- `!play [URL/search term]` - Play a song from YouTube or Spotify.
- `!pause` - Pause the current song.
- `!resume` - Resume playback.
- `!stop` - Stop playback, clear the queue, and leave the voice channel.
- `!skip` - Skip the current song.
- `!queue` - Show the current song queue.
- `!leave` - Leave the voice channel.
- `!loop` - Toggle loop mode for the current song.
- `!log` - Log the current context.
- `!restart` - Restart the bot (Owner only).
- `!logclear` - Clear the log file (Owner only command).
- `!nowplaying` - Show the currently playing song.

## Troubleshooting
- **FFmpeg Installation**: Ensure `ffmpeg` is in your system's PATH. If issues persist, manually download and place `ffmpeg` in the bot's root directory.
- **Bot Token Issues**: Double-check that the Discord bot token is correctly placed in the `.env` file.
- **Please Sign-In YouTube Issue**: Your cookies.txt file may be either invalid, missing or expired. Export it as .json 

For further assistance, please refer to the bot's documentation or open a Issue on GitHub.