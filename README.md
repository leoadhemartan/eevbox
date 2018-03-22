# eevbox (EasyEngine Vagrant Box)

This is my customized Vagrant VirtualBox machine that I use for local web development and testing. It uses EasyEngine to set everything up.

The box used in the Vagrantfile is customized according to my preference and workflow but anyone who just wants a working nginx server for WordPress on the localhost will find this useful.

Using this box requires that you install [Vagrant](https://www.vagrantup.com/) and [VirtualBox](http://virtualbox.org/)

It also requires that you are at least comfortable with using a terminal.

I use [MobaXterm](https://mobaxterm.mobatek.net/) to access the box but any terminal client will do.

## Setting Up

Load the Vagrantfile and the .vagrant folder to your preferred location.

Customize the Vagrantfile according your preferences.

Update your hosts file for ee.vm and point it to the Private Network ip set in the Vagrantfile.

## Starting the box

Start PowerShell or cmd.

Go to the folder where the Vagrantfile and .vagrant folder is located.

Run 

```Bash
vagrant up --provision
```

Once vagrant confirms that your box is up and running, open http://ee.vm to confirm. If a page loads, your EasyEngine Vagrant VirtualBox machine is now running.

## Access details

### ssh

username: vagrant
password: vagrant

### sftp

username: www-data
password: vagrant

#### EasyEngine commands can be found at https://easyengine.io/