# mpv-settings-gpu-next
My personal config for MPV media player. This config uses by default gpu-api vulkan and vo=gpu-next and may not be suitable for your device. If you have any recommendations, just get in touch with me (Discussions) or create a pull request.

# Installation
Depending on your Operating System, you need to place the stuff inside the zip in a certain directory.
The root directory needs to look like this (Should be considered a Tree View example):


>Roaming

>>mpv

>>input.conf

>>mpv.conf

>>>shaders

>>>script-opts

>>>scripts

>>>fonts

## WINDOWS INSTALLATION
> "C:\Users\ %Username% \AppData\Roaming\mpv"

## MAC INSTALLATION
Path:

/USERNAME/.config/mpv

## LINUX INSTALLATION

Path:
~/.config/mpv

Flatpak:
~/.var/app/io.mpv.Mpv/config/mpv


# Documentation
## Scaler & Shader used: 

- RAVU: https://github.com/bjin/mpv-prescalers
- SSimSuperRes: https://gist.github.com/igv/2364ffa6e81540f29cb7ab4c9bc05b6b
- SSimDownscaler: https://gist.github.com/igv/36508af3ffc84410fe39761d6969be10
- GLSL Chroma from Luma (CfL) Prediction: https://github.com/Artoriuz/glsl-chroma-from-luma-prediction

#### Comparison: https://artoriuz.github.io/blog/mpv_upscaling.html

## List of Scripts used:
- acompressor.lua - Dynamic range compressor using acompressor ffmpeg filter with controls to dynamically adjust parameters.
- autocrop.lua - Automatically crop the video by using lavfi's cropdetect filter to detect black bars. Press 'C' (Shift+c) to activate.
- autoload.lua - preloads all files in a folder into a playlist.
- auto-save-state.lua - Periodically saves progress with write-watch-later-config, and also cleans up the watch later data after the file is finished playing (so playlists may continue at the correct file).
- pause-when-minimize.lua - Pauses the player video when minimizing, and unpauses it when brought up again.
- playlistmanager.lua - This script allows you to see and interact with your playlist in an intuitive way.
- quality-menu.lua - Allows you to change the streamed video and audio quality (ytdl-format) on the fly. 
- quality-menu-osc.lua - enables UI integration for default OSC
- status-line.lua - Rebuild the terminal status line as a lua script

# Troubleshooting

If you have issues with my settings, create a new issue on this github page but please first go through the mpv.conf, most of it is self-explanatory due to the comments.

# Credits
- https://iamscum.wordpress.com/guides/videoplayback-guide/mpv-conf/
- https://github.com/Tsubajashi/mpv-settings
- https://github.com/xzpyth/mpv-config
- https://kohana.fi/article/mpv-for-anime
- https://github.com/classicjazz/mpv-config
