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

- FSRCNNX_x2_8-0-4-1.glsl: https://github.com/igv/FSRCNN-TensorFlow/releases
- SSimSuperRes.glsl: https://gist.github.com/igv/2364ffa6e81540f29cb7ab4c9bc05b6b
- SSimDownscaler.glsl: https://gist.github.com/igv/36508af3ffc84410fe39761d6969be10
- KrigBilateral.glsl: https://gist.github.com/igv/a015fc885d5c22e6891820ad89555637
- ravu-zoom-r3/r4.hook: https://github.com/bjin/mpv-prescalers
- adaptive-sharpen.glsl: https://gist.github.com/igv/8a77e4eb8276753b54bb94c1c50c317e
- FSR.glsl: https://gist.github.com/agyild/82219c545228d70c5604f865ce0b0ce5  

#### Comparison: https://artoriuz.github.io/blog/mpv_upscaling.html

## List of Scripts used:

- Mac_Integration.lua - This script enables a few shortcuts which Mac users are familiar with. See scripts/Mac_Integration.lua for more infos.
- acompressor.lua - a simple audio compression script which can normalize your audio of the files played with mpv. See scripts/acompressor.lua for more infos.
- appendURL.lua - when mpv is opened, you can copy paste a URL in to play from.
- audio-osc.lua - different on screen controls for audio-only playback.
- autoload.lua - preloads all files in a folder into a playlist.
- seek-to.lua - when "t" is pressed, you can seek to a specific part of the video/audio you are currently watching.
- webm.lua - Simple WebM maker for mpv. By default, the script is activated by the W (shift+w) key.
- playlistmanager.lua - This script allows you to see and interact with your playlist in an intuitive way. SHIFT+ENTER = playlist
- quality-menu.lua - Allows you to change the streamed video and audio quality (ytdl-format) on the fly. Simply open the video or audio menu, select your prefered format and confirm your choice. The keybindings for opening the menus are configured in input.conf, and everthing else is configured in quality-menu.conf. By default: List Video Formats: F (shift+f), List Audio Formats: Alt+f, Reload: Ctrl+r. 
- quality-menu-osc.lua - enables UI integration for default OSC

# Troubleshooting

If you have issues with my settings, create a new issue on this github page but please first go through the mpv.conf, most of it is self-explanatory due to the comments.

# Credits
- https://iamscum.wordpress.com/guides/videoplayback-guide/mpv-conf/
- https://github.com/Tsubajashi/mpv-settings
- https://github.com/xzpyth/mpv-config
- https://kohana.fi/article/mpv-for-anime
- https://github.com/classicjazz/mpv-config
