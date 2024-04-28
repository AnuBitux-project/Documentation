# How to update an AnuBitux VM

The AnuBitux VM has been designed to work in a more permanent way, even to perform only test and trainings. To update the distro and the tools there is a dedicated script in the same GitHub repository, named&#x20;

```
update_vm.sh
```

Before running it, it is necessary to update the version of the tools in the variables at the beginning of the script. If the script has been updated in the GitHub repository, it is enough to move to the script's directory with the terminal and type

```
git pull
```

If the GItHub repository is not fully up to date, it is necessary to check manually the version of each tool before running the script.
