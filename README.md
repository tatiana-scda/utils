        Log out
        Hit Ctrl+Alt+F1 and login using your credentials.
        kill your current X server session by typing 
        sudo service lightdm stop
        Enter runlevel 3 by typing 
        sudo init 3
        Go to directory and check the file in there (cd Downlods; ls NVIDIA*)
        Make the file executable with 
        chmod +x ./your-nvidia-file.run
        Execute the file with 
        sudo ./your-nvidia-file.run
        If not required to reboot, run 
        sudo service lightdm start
