# How to build AnuBitux

AnuBitux is a distro designed to handle very sensible information so it tries to be as more trustless as possible. SI, if a user doesn't want to download the builded iso or does not trust the building logs published on the [Download page](https://anubitux.org/download-anubitux/), it is also possible to self build it following these simple steps (also shown [here](https://github.com/AnuBitux-project/build)):

* Use a Debian-based working environment for the building process;
* Install dependencies

```
sudo apt install live-build squashfs-tools syslinux-common syslinux-utils xorriso isolinux
```

* Create a folder

```
mkdir distro
```

* Move your terminal into the folder

```
cd distro
```

* Configure the parameters

```
lb config -b iso -d bookworm --cache true --apt-recommends true -a amd64 --binary-images iso --debian-installer none --linux-flavours amd64 --mode debian --debian-installer-gui false --archive-areas "main contrib non-free non-free-firmware" --security true --win32-loader false --interactive shell --updates true --iso-application anubitux --iso-publisher https://anubitux.org --iso-volume anubitux --memtest none --bootappend-live "boot=live config hostname=AnuBitux username=anubitux"
```

* Obtain root privileges

```
sudo -s
```

* Launch the building process

```
lb build
```

* Copy the anubitux\_script.sh file to the chroot&#x20;

```
sudo cp anubitux_script.sh /home/$USER/distro/chroot/
```

* Execute the script (if needed, edit the versions of the tools at the beginning of the script file)

```
chmod +x anubitux_script.sh
./anubitux.sh
```

* Configure the last files, for example the building date, and clean the command history

```
nano /opt/scripts/Info.sh
history -c
```

* Type exit to start the building process

```
exit
```

* Wait until it ends

When the process finishes, the _.iso_ file can be found in the above created distro folder. To be sure it runs on a bootable USB, it may be necessary to run this command.

```
isohybrid isofilename.iso
```



