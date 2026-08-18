# Warehouse Standalone Server


<p>
    Compatible to 
    <a href="https://github.com/MichaelFedorchenko/warehouse/releases/tag/v1.7">
        <img src="https://img.shields.io/badge/Warehouse%20Desktop%20Application-v1.7.1-orange" height=25>
    </a>
</p>


> Package to install: warehouse-server.deb

### Application files:
```
/opt/warehouse/photos/           Derectory for photos
/opt/warehouse/settings.json     Application Settings
/opt/warehouse/warehouse.db      Database (SQLite)
/opt/warehouse/warehouse-server  Main Server Application
```

### Daemon
```
/lib/systemd/system/warehouse-server.service
```

### Application Settings (file: /opt/warehouse/settings.json)
```
{
  "db_path": "/opt/warehouse/warehouse.db",
  "show_content": false,
  "photos_dir": "/opt/warehouse/photos",
  "language": "en",
  "admin_password": "12345",
  "port": 4300,
  "host": "0.0.0.0"
}
```

### Describe of setings
```
db_path       [string]    Current Database file
show_content  [boolean]   Show Items-name in Container for GUI-App (Default: false)
photos_dir    [string]    Current Photos Directory
language      [string]    Current Application Language (Default: "en")
  You can change language:
  ge - german
  en - English
  sp - Spanish
  fr - French
  it - Italian
  pl - Polish
  ua - Ukrainian
admin_password  [string]  Current password for Admin panel (Default: 12345)
port            [integer] Current Server Port (Default: 4300)
host            [string]  0.0.0.0 For everyone / 127.0.0.1 - for local use
```
