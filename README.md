# Fix slow startup ubuntu virtual machines

Sometimes I have experienced a startup that is too slow on Ubuntu virtual machines, for this reason to solve this case I have the following changes once the Ubuntu operating system has been installed on a virtual machine.

```bash
sudo apt update
sudo apt full-upgrade
````

```bash
sudo apt install gcc make perl
sudo apt install build-essential linux-headers-$(uname -r)
sudo apt update
sudo add-apt-repository multiverse
sudo apt update
sudo apt install virtualbox-guest-utils virtualbox-guest-x11
````

And now we have to rebbot the system.

```bash
sudo reboot
````

And now we can install the **Guest additions** from **VirtualBox**
