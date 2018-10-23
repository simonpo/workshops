# Connecting to an Azure VM from a Mac

## Connecting to a Windows DSVM
Follow the instructions [here](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/connect-logon).

You will need to install an RDP client for Mac such as [Microsoft Remote Desktop](https://itunes.apple.com/app/microsoft-remote-desktop/id715768417).

## Connecting to an Ubuntu DSVM

### SSH
Use the in-built Terminal to connect to your Ubuntu VM over SSH. 
1. Open Applications > Utilities, and then open Terminal 
1. At the command prompt, enter:

``` bash
ssh username@ipaddress
```

replacing ```username``` with your user name, and ```ipaddress``` with the IP address of your VM.