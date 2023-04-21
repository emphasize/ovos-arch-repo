# ovos-arch-repo
OpenVoice OS Arch Packages Repository

#### How To Use OVOS Arch Repository
Platforms Supported: x86_64, aarch64(Arm64)

**Edit Pacman.conf to add OVOS Repository**
```
sudo nano /etc/pacman.conf
```

**Add OVOS Repository Entry**
**Make sure it matches the following - Copy/Paste As Given**
```
[ovos-arch-repo]
SigLevel = Optional DatabaseOptional
Server = https://github.com/OpenVoiceOS/ovos-arch-repo/raw/main/$arch
```

**Sync and Update**
```
sudo pacman -Sy
```

**Install a package**
```
sudo pacman -S python-ovos-core
```

**Install Full Build**
```
sudo pacman -S ovos-install-meta-full
```
