# MiniDLNA

### Installation
`apt-get install minidlna`

### Reference
[MiniDLNA](https://help.ubuntu.com/community/MiniDLNA)

### Configuration
  + File Path<p>
    `/etc/minidlna.conf`<p>

  + Configuration Globally (for all users)
  ```
    #network_interface=eth0         # Self-discovers if commented (good with NetworkManager)
    media_dir=A,/home/user/Music    # Use A, P, and V to restrict media 'type' in directory
    media_dir=P,/home/user/Pictures
    media_dir=V,/home/user/Videos
    friendly_name=Laptop            # Optional, a name for users to see
    db_dir=/var/cache/minidlna      # Needs to be un-commented
    log_dir=/var/log                # Needs to be un-commented
    inotify=yes                     # 'no' for less resources, restart required for new media
  ```
  PS:
  ```
    # Restart the daemon for changes to take effect:
    service minidlna restart

    # To rebuild the database use:
    service minidlna force-reload
  ```

  + Configuration Locally (per user)<p>
  see [MiniDLNA](https://help.ubuntu.com/community/MiniDLNA)<p>
