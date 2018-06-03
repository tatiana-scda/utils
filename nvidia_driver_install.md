Log out
Ctrl+Alt+F1 and login using credentials

kill X server session 
```
sudo service lightdm stop
```

Enter runlevel 3
```
sudo init 3
```

Go to directory and check the file (ls NVIDIA*)

Make the file executable
```
chmod +x ./your-nvidia-file.run
```

Execute the file
```
sudo ./your-nvidia-file.run
```

If not required to reboot, run 
```
sudo service lightdm start
```
