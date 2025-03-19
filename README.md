# radiostreamer

A lightweight Bash script for streaming audio from internet radio stations. It is an easy to use tool for streaming internet radio from various sources and piping the progamming through VLC or MPV. It is an improvement over the [VLC-Playlist](https://github.com/AB9IL/Skywave-Linux-v4/blob/master/vlc-playlist) script in Skywave Linux version 4. Set up a playlist file, then pick internet radio stations to stream. Edit the playlist to add or remove entries.

#### Dependencies:

All dependencies are probably in your distro's software repositories. If not, go get them and compile what you need:

- CVLC, MPV, or ffplay
- Rofi or Dmenu
- Fzf
- Yad

#### What the Radiostreamer Does:

Reads playlist of streaming audio broadcasters and presents a "fuzzy finder" style menu.  When a sation is selected, the application drops into the backgound to provide audio.  Bring up the menu again to select another station or stop streaming.  Amplitude compression is enabled by default to to make loudness more consistent across the various streams.

#### Installation:

Clone the repository, place the script within your system's path. Move the playlist to your home/.config directory. Place the launcher in your home/.local/share/applications directory (or wherever you keep your launchers). The playlist is contained in the file "radiostreams" and it is normally kept in the ~/.config directory.  Entries are one line per stream, comma separated: url,name of the station. Edit the list as necessary, because stream urls do occaisionally change.

#### Usage:
Launch it from the command line with either _"radiostreamer gui_" or _"radiostreamer"_ to get the menu in Rofi or Fzf, respectively. Choices will be to pick a station for streaming, stop streaming, or edit the playlist.
