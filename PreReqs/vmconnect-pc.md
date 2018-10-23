# Connecting to an Azure VM from a Windows PC

## 1. Connecting to a Windows DSVM
You don't need to install any additional software on your laptop.

Follow the instructions to set up a Remote Desktop Connection from your local Windows PC to a remote Windows VM [here](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/connect-logon).

## 2. Connecting to an Ubuntu DSVM
You can connect to your Ubuntu VM using either SSH for command line access, or X2Go if you want a full graphical desktop. If you're comfortable with a command line interface, we recommend just using SSH to connect to your machine. 

### 2.1 SSH
We recommend that you use Putty as your SSH client:

* [Putty](https://www.putty.org/)

### 2.2 X2Go
If you prefer a graphical desktop (X Windows System), you can install the X2Go client. The Linux VM is already provisioned with X2Go server and ready to accept client connections.

* Download and install the [X2Go client](https://wiki.x2go.org/doku.php/doc:installation:x2goclient) for your client platform from X2Go.
* Run the X2Go client, and select New Session. It opens a configuration window with multiple tabs. Enter the following configuration parameters:

* Session tab:
  * Host: The host name or IP address of your Linux Data Science VM.
  * Login: User name on the Linux VM.
  * SSH Port: Leave it at 22, the default value.
  * Session Type: Change the value to XFCE. Currently the Linux VM only supports XFCE desktop.
* Media tab: If you don't need to use sound support and client printing, you can turn them off.
* Shared folders: If you want directories from your client machines mounted on the Linux VM, add the client machine directories that you want to share with the VM on this tab.

After you sign in to the VM by using either the SSH client or XFCE graphical desktop through the X2Go client, you are ready to start using the tools that are installed and configured on the VM.