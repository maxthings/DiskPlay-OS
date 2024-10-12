# DiscPlay OS

DiscPlay OS is a lightweight, Linux-based operating system designed for laptops to function as a dedicated DVD/CD/Blu-ray player with additional smart TV-like capabilities. Along with disc playback, it supports streaming services, media servers, and USB playback, providing a complete home media experience.

## Features

- **Disc Playback**: Native support for DVD, Blu-ray, and CD playback with auto-detection.
- **Streaming Services**: Access Netflix, YouTube, Disney+, and other streaming platforms directly from the OS.
- **Media Server Integration**: Connect to media servers like Plex, Jellyfin, and more to stream your media library.
- **USB Support**: Automatically detect and play media files from connected USB devices.
- **TV-Like Interface**: Intuitive, remote-friendly interface with a simple home screen and app launcher.
- **Internet Access**: Full support for internet browsing and online apps.
  
## Screenshots
(Add screenshots of the UI here)

## Requirements

- Laptop with a DVD/CD/Blu-ray drive
- Minimum 2GB RAM, 20GB storage
- Wi-Fi or Ethernet connection for internet access
- USB ports for external storage

## Installation

1. **Download the ISO**: 
    Download the latest version of the DiscPlay OS ISO from the [releases page](https://github.com/your-username/discplay-os/releases).
    
2. **Create a Bootable USB**:
    Use a tool like [Rufus](https://rufus.ie/) (Windows) or `dd` (Linux) to create a bootable USB drive.
    - Example using `dd`:
      ```bash
      sudo dd if=DiscPlay-OS.iso of=/dev/sdX bs=4M
      ```
      
3. **Install on Your Laptop**:
    - Boot from the USB and follow the installation steps.
    - Once installed, the OS will boot directly into the media playback interface.

## Usage

### Playing Discs
- Insert a DVD, Blu-ray, or CD, and the media will automatically play via the built-in media player (VLC).
  
### Streaming Apps
- Access Netflix, YouTube, Disney+, and more via the pre-installed web browser in fullscreen mode.
  
### Connecting Media Servers
- Open the **Media Server** app to connect to your Plex or Jellyfin server and stream your library.
  
### USB Media Playback
- Insert a USB drive, and the OS will detect media files automatically. Use the media player to browse and play your content.

### TV-Like Interface
- The OS features a home screen similar to a smart TV. Use arrow keys or a remote to navigate between apps and media options.

## Customization

- **Home Screen**: Modify the home screen layout via the settings menu.
- **App Shortcuts**: Add or remove streaming app shortcuts for faster access.

## How to Build

For developers looking to contribute or modify the OS:

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/maxthings/discplay-os.git
    ```

2. **Build the ISO**:
    After making your changes, use the `live-build` tool to generate a new ISO:
    ```bash
    sudo apt install live-build
    cd discplay-os
    sudo lb build
    ```

3. **Contributing**:
    Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Troubleshooting

- **No Disc Detected**: Ensure that your DVD/Blu-ray drive is connected properly and supported by VLC.
- **Network Issues**: Check your Wi-Fi or Ethernet connection if streaming apps are not working.
  
## Roadmap

- Adding support for additional streaming services.
- Voice control integration.
- Smart remote support.

## License

DiscPlay OS is open-source and licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

---

### Support

If you have any issues or questions, feel free to open an issue or reach out to the community for help.
