These patches are for building gentoo's official repo app-emulation/virtualbox packages for linux kernel 5.0.0-rc1 (and possibly later)

##Copy Patches
```
cd ~/
git clone https://github.com/aesycos/Patches.git
cd Patches/gentoo/app-emulation/virtualbox-modules-6.0.0/
sudo mkdir -p /etc/portage/patches/app-emulation/virtualbox-modules-6.0.0
cp * /etc/portage/patches/app-emulation/virtualbox-modules-6.0.0/
```
##Enable unstable app-emulation/virtualbox ebuilds
```
echo "app-emulation/virtualbox ~amd64\napp-emulation/virtualbox-modules ~amd64" >> /etc/portage/package.accept_keywords
```

##Installing
```
emerge -aq1 app-emulation/virtualbox
```

(Be sure that portage is trying to emerge virtualbox 6.0.0)

##Cleanup
```
cd ~/
rm -rf Patches
```
