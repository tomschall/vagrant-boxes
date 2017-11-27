# Vagrant Base Boxes

## Downloads

* **[CentOS-7-x86_64-v20171127.box](https://www.dropbox.com/s/4yk8dhopfk6cwoe/CentOS-7-x86_64-v20171127.box):** CentOS 7 x86\_64 Minimal *(VirtualBox 5.0.20 Guest Additions)*  
  <small>sha256sum: `cf92ef32edf0f8e4ab45bcab1bc79277f58c67ff86aab55b5230199297cfffb5`</small>

## How these boxes were built

These boxes were automatically built using [packer](http://www.packer.io) (v1.1.2) and the definitions in this repo:

```sh
$ cd packer
$ ./build.sh
```

The definitions are based on the [veewee project's](https://github.com/jedi4ever/veewee) definitions for a minimal CentOS installation, but with a few modifications:

- The disk can grow to 200GB
- Provides 4GB of swap
- Provides 1024 MB of RAM
- Fixes [slow DNS resolution](https://github.com/NREL/vagrant-boxes/issues/5)
