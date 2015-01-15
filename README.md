# mac-os-tips
A collection of useful things concerning Mac OS X

### Slow Terminal Login and Cleaning Log Files ###

If you are experiencing that it takes a long time to open a new login shell, one reason could be the accumulation of system log files in the directory 

    /private/var/log/asl/
    
![](./images/terminal_login_1.png)
![](./images/terminal_login_2.png)

In my case, I could bring my terminal back to speed by simply deleting those `.asl` log files via:

	cd /private/var/log/asl/
	sudo rm *.asl 
