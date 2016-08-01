# MiniDLNA

### Installation
`apt-get install minidlna`

### Configuration
  + File Path
    `/etc/minidlna.conf`

  + Configure
  ```
    #network_interface=eth0         # Self-discovers if commented (good with NetworkManager)
    media_dir=A,/home/user/Music    # Use A, P, and V to restrict media 'type' in directory
    media_dir=P,/home/user/Pictures
    media_dir=V,/home/user/Videos
    friendly_name=Laptop            # Optional
    db_dir=/var/cache/minidlna      # Needs to be un-commented
    log_dir=/var/log                # Needs to be un-commented
    inotify=yes                     # 'no' for less resources, restart required for new media
  ```
