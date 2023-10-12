![Melawy Linux](/profile/Melawy_Linux_640x320.svg?raw=true)

Melawy Linux - это как независимая разработка программ и оформления, так и замствование интересных идей. 

Продукт является открытым программным обеспечением со свободной лицензией. 

Проект нацелен на сегмент ПК и ноутбуков. 

Приглашаем энтузиастов для совместной разработки, тестирования программ и оформления.

---

Скачать и подписать ключ как доверенный

```bash
sudo pacman-key --recv-keys 95F48000540A4DB146583A47C49B5E77FD80302D --keyserver hkps://keys.openpgp.org
sudo pacman-key --lsign-key 95F48000540A4DB146583A47C49B5E77FD80302D
```

или

```bash
sudo pacman-key --lsign-key 95F48000540A4DB146583A47C49B5E77FD80302D --keyserver http://keyserver2.pgp.com
sudo pacman-key --lsign-key 95F48000540A4DB146583A47C49B5E77FD80302D
```

Вставить в /etc/pacman.d/melawy-linux-mirrorlist 
следующее содержимое:

```
######################################################
####                                              ####
###       Melawy Linux Repository Mirrorlist       ###
####                                              ####
######################################################
#### Entry in file /etc/pacman.conf:
###    [melawy]
###    SigLevel = Required DatabaseOptional
###    Include = /etc/pacman.d/melawy-linux-mirrorlist
###
###    [melawy-aur]
###    SigLevel = Required DatabaseOptional
###    Include = /etc/pacman.d/melawy-linux-mirrorlist
###
###    [melawy-aur-kde]
###    SigLevel = Required DatabaseOptional
###    Include = /etc/pacman.d/melawy-linux-mirrorlist
###
###    [melawy-aur-theme]
###    SigLevel = Required DatabaseOptional
###    Include = /etc/pacman.d/melawy-linux-mirrorlist
###
###    [melawy-aur-gui-app]
###    SigLevel = Required DatabaseOptional
###    Include = /etc/pacman.d/melawy-linux-mirrorlist
###
######################################################

Server = https://github.com/Melawy/$repo-repo/raw/main/$arch/
```

Добавить в /etc/pacman.conf

```
[melawy]
SigLevel = Required DatabaseOptional
Include = /etc/pacman.d/melawy-linux-mirrorlist

[melawy-aur]
SigLevel = Required DatabaseOptional
Include = /etc/pacman.d/melawy-linux-mirrorlist

[melawy-aur-kde]
SigLevel = Required DatabaseOptional
Include = /etc/pacman.d/melawy-linux-mirrorlist

[melawy-aur-theme]
SigLevel = Required DatabaseOptional
Include = /etc/pacman.d/melawy-linux-mirrorlist

[melawy-aur-gui-app]
SigLevel = Required DatabaseOptional
Include = /etc/pacman.d/melawy-linux-mirrorlist
```

Выполнить

```bash
sudo pacman -Sy
sudo pacman -S melawy-linux-mirrorlist melawy-linux-keyring --overwrite="*"
```

---
### Смотреть видео

[![Watch video](https://i3.ytimg.com/vi/bRNVm1VIxbA/maxresdefault.jpg)](https://www.youtube.com/watch?v=bRNVm1VIxbA)

---

![](/profile/01.jpg?raw=true)
![](/profile/02.jpg?raw=true)
![](/profile/03.jpg?raw=true)
![](/profile/04.jpg?raw=true)
![](/profile/05.jpg?raw=true)
![](/profile/06.jpg?raw=true)
![](/profile/07.jpg?raw=true)
![](/profile/08.jpg?raw=true)
![](/profile/09.jpg?raw=true)
![](/profile/10.jpg?raw=true)
![](/profile/11.jpg?raw=true)
![](/profile/12.jpg?raw=true)
![](/profile/13.jpg?raw=true)
![](/profile/14.jpg?raw=true)
![](/profile/15.jpg?raw=true)
![](/profile/16.jpg?raw=true)

---

Melawy Linux использует в качестве основы Arch Linux, сборку через ArchISO, установку через Calamares. 

Репозитории: 
- core
- extra
- community
- multilib
- xhbp
- xiso
- xerolinux_repo
- xerolinux_repo_xl
- arcolinux_repo
- arcolinux_repo_xlarge
- arcolinux_repo_3party
- cachyos
- garuda
- chaotic-aur
- endeavouros
- melawy
- melawy-aur
- melawy-aur-kde
- melawy-aur-theme
- melawy-aur-gui-app

Системные компоненты: 
- refind
- btrfs
- efi
- vmlinuz + initrd
- ukify
- dracut
- systemd 253+
- timeshift
- plymouth
- sddm
- kde
- pipewire

Пакетные менеджеры: 
- pacman
- pamac
- paru
- yay
- octopi

Обновление зеркал пакетов: 
- Reflector
- Reflector simple

Стандартный набор программ: 
- LibreOffice
- OnlyOffice
- Firefox
- Firefox Dev
- Chrome
- Telegram
- Discord
- VS Code
- Zoom
- Skype
- KeePassXC
- YandexDisk
- AnyDesk

Графические редакторы: 
- Gimp
- InkScape
- Krita

Мультимедиа: 
- ObsStudio with Browser support
- Haruna
- Vlc
- Mpv
- Elisa
- Audacious
- Audacity
- Avidemux

Почта: 
- Mailspring
- Thunderbird

При необходимости можно установить:
- Brave
- Opera
- WhatsApp
