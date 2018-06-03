Fuse is a free option for writing files in NTFS disk

Install xcode
```
xcode-select --install
```

install homebrew
 ```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

install fuse
```
brew cask install osxfuse
```

you can manually mount a partition
```
sudo mkdir /Volumes/NTFS
```

list all disks
```
diskutil list
```

unmount it (OS will mount when plug)
```
sudo umount /dev/disk2s1
```

mount it properly
```
sudo /usr/local/bin/ntfs-3g /dev/disk2s1 /Volumes/NTFS -olocal -oallow_other
```
