# RBox
A virtual root filesystem for Android devices.

## Installing
1. Download a terminal emulator ror Android. We reccommend to use [Jack Palevich's Terminal Emulator.](https://play.google.com/store/apps/details?id=jackpal.androidterm)
2. Download the latest [setup file.](http://dl.litesec.co/projects/rbox/rbox-setup)
3. Start the termina emulator (Assuming you are using JP's Terminal Emulator)
4. Navigate to the terminals data directory, located at ```/data/data/jackpal.androidterm```.
5. Use ```cp <path-to-setup-file> $PWD``` to copy the installer to data directory.
6. Execute the following commands to install RBox:

> ``` chmod 775 rbox-setup ```

> ``` ./rbox-setup ```

If the installer completes successfully, you should get a similar output to this:

> The full path of the RBOX shell is ./rbox/bin/rbox_shell

NOTE: If you get 'Permission denied' error when running the last command, try executing ```chmod +x rbox-setup``` and try again.

### Optional
After the installation, there are some optional actions available. They won't affect the performance/functionality of the system, but will definitely improve the user experience.

##### 1. Remove the installation files
Assuming you are still located in the terminal data directory, execute this command:

> ```rm rbox-setup-* -rf```

##### 2. Make RBOX the default shell

JP's Terminal Emulator has a neat feature, which allows you to specify the default shell program you want to use, in this case it is ```rbox-shell```. If you use this option, you wont have to manualy type the location of the shell every time you start the terminal.

1. Start the Terminal Emulator, press the 3 dots at the top right corner, and select the ```Preferences``` option.

2. Scroll down and under the ```Shell``` tab, select ```Command line```
3. Replace the default command line with the location of rbox_shell. If you followed our guide, the path should be ```/data/data/jackpal.androidterm/rbox/bin/rbox_shell```

4. Relaunch the Terminal Emulator to apply the settings.
