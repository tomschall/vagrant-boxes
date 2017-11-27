## v20171127 / 2017-11-27

* Switch build process to use [Packer](http://www.packer.io) for increased automation.
* Improve Vagrant sudo setup so changes to `/etc/sudoers` don't accidentally enable `requiretty`, breaking Vagrant sudo usage.
* Fix slow DNS resolution when VirutalBox's DNS proxy is used (the default). Fixes [#5](https://github.com/NREL/vagrant-boxes/issues/5).
* Increase available swap to 4GB
* Software Versions
  * CentOS 7
  * VirtualBox Guest Additions 5.0.20
