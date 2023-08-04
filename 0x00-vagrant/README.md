# VAGRANT VIRTUAL ENVIRONMENT
This file describes the process of installing virtualbox and vagrant in Linux
NOTE: This installation process was tested on kali linux

## Installing virtualbox
Virtualbox is a virtualization software developed by Oracle. It provides the virtual environment on top of your primary operating system, the host, where a virtual OS, the guest, is installed and run from. This virtual machine environment is isolated from you host OS ensuring no interference between the two OSs as they don't know anything about each others' existence.
```
sudo apt install -y virtualbox virtualbox-ext-pack
``` 
Click on [this link](https://www.kali.org/docs/virtualization/install-virtualbox-host/ "Installing virtualbox in Kali Linux") for a step-by-step process on how to install virtualbox on Kali Linux

## Installing vagrant
Vagrant is an open-source tool for working with virtual machines. It builds and maintains virtual software development environments on providers like VirtualBox, KVM, Hyper-V, Docker containers among others. 
```
sudo apt-get install vagrant
```
Click on [this link](https://installati.one/install-vagrant-kalilinux/?expand_article=1 "Vagrant installation")   to learn more about installing vagrant on Kali Linux

## Why The Installation?
The aim is to create a virtual development environment in my/your local machine which is similar to the one used to run code tests in the cloud.

## Creating your virtual machine
This virtual machine will be running Ubuntu 20.04 LTS
After installing both softwares in the above steps, run the commands below in your terminal to create and interact with your virtual machine
* `vagrant init ubuntu/focal64` - This generate a vagrant file. You only need to run this command once during the creation of your VM.
* `vagrant up` - Start and provision your virtual machine
* `vagrant ssh` - Connects to virtual machine via ssh
* When done with your virtual machine, type `exit` to go back to your host machine terminal
* `vagrant reload` - restarts the vagrant machine and loads new Vagrantfile configuration
* `vagrant resume` - resumes a suspended vagrant machine

Run `vagrant --help` to view more vagrant commands and other helpful information.

If you have come this far, congratulations for setting up your virtual machine environment!


