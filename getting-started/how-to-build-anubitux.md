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
* Obtain root privileges
* Launch the building process
* Copy the anubitux\_script.sh file to the chroot&#x20;
* Execute the script (if needed, edit the versions of the tools at the beginning of the script file)
* Configure the last files
* Type exit to start the building process
* Wait until it ends

Use a Debian working environment for the building process.

