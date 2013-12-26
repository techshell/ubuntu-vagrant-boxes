##Description

Create your very own vagrant base boxes using [packer](http://www.packer.io).

* All boxes are 64 bit.
* All boxes include the latest VirtualBox Guest Additions installed.
* All boxes include the latest Chef 11.x client [installed](http://www.getchef.com/chef/install/).

##Requirements

* [vagrant](http://vagrantup.com)
* [packer](http://packer.io)
* [virtualbox](https://www.virtualbox.org/)


##Installation

1. Make sure you have packer [installed](http://www.packer.io/intro/getting-started/setup.html).
2. To create a base box, cd to the relevant folder and run the command `packer build <distro>.json`.
3. Wait a while for the base box to built, the final box file will be saved to the `build/<distro>.box`.
4. Finally you can add the base box to vagrant by running `vagrant box add {title} <distro>.box`

##Available boxes

Release | Codename | Download
--- | --- | ---
[Ubuntu 12.04 Server](http://releases.ubuntu.com/12.04/) | Precise Pangolin | [Link](http://copy.com/WQTmzQY1UOHG/vagrant/precise64.box)
[Ubuntu 12.10 Server](http://releases.ubuntu.com/12.10/) | Quantal Quetzal | [Link](http://copy.com/WQTmzQY1UOHG/vagrant/quantal64.box)
[Ubuntu 13.04 Server](http://releases.ubuntu.com/13.04/) | Raring Ringtail | [Link](http://copy.com/WQTmzQY1UOHG/vagrant/raring64.box)
[Ubuntu 13.10 Server](http://releases.ubuntu.com/13.10/) | Saucy Salamander | [Link](http://copy.com/WQTmzQY1UOHG/vagrant/sausy64.box)

###How To Use

```
$ vagrant box add {title} {link}
$ vagrant init {title}
$ vagrant up
```

##License

Copyright: 2014, Hatim Abdalla.
Licensed under The MIT License.
