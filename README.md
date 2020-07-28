# Burp Autostart Service
Service script for auto starting Burp (Backup and Restore Program).
Useful for systems using Systemd.

This is just a compilation, the original file is from: https://aur.archlinux.org/cgit/aur.git/tree/?h=burp-backup.

Thanks to Graham Keeling (the author of Burp) for pointing me there.

## How To Use
-Download the file.

-Move it to "/etc/systemd/system/"
```
sudo mv burp-server.service /etc/systemd/system/
```

-Give it permissions:
```
sudo chmod 664 /etc/systemd/system/burp-server.service
```

-Enable it
```
sudo systemctl daemon-reload
sudo systemctl enable burp-server.service
```

## Burp
Burp is a network backup and restore program. It attempts to reduce network traffic and the amount of space that is used by each backup. 

Link: https://burp.grke.org/

