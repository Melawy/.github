![Melawy Linux](/profile/Melawy_Linux_640x320.svg)

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
###    [melawy-aur-cargo]
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

[melawy-aur-cargo]
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

[![Watch video](https://i3.ytimg.com/vi/gV-4n7IcDdc/maxresdefault.jpg)](https://www.youtube.com/watch?v=gV-4n7IcDdc)

---

![](/profile/01.jpg)
![](/profile/02.jpg)
![](/profile/03.jpg)
![](/profile/04.jpg)
![](/profile/05.jpg)
![](/profile/06.jpg)
![](/profile/07.jpg)
![](/profile/08.jpg)
![](/profile/09.jpg)
![](/profile/10.jpg)
![](/profile/11.jpg)
![](/profile/12.jpg)
![](/profile/13.jpg)
![](/profile/14.jpg)
![](/profile/15.jpg)
![](/profile/16.jpg)

---

Melawy Linux использует в качестве основы Arch Linux, сборку через ArchISO, установку через Calamares. 

Репозитории: 
- core
- extra
- community
- multilib
- arcolinux_repo
- arcolinux_repo_xlarge
- arcolinux_repo_3party
- melawy
- melawy-aur
- melawy-aur-gui-app
- melawy-aur-theme
- melawy-aur-kde
- melawy-aur-cargo
- AUR

Не используются специфичные для ArcoLinux программы и оформление.

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
- Vlc
- Mpv
- Elisa
- Audacious
- Audacity
- Avidemux

Почта: 
- Mailspring
- Thunderbird
- Kube

При необходимости можно установить:
- Brave
- Opera
- WhatsApp
