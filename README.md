# CakeOven Box

This machine is supposed to be a version of Laravel Homestead for CakePHP v3.


## Building the box

1. Install [Packer](https://www.packer.io/downloads.html)
2. Run ```packer build template.json```


## Variables
All the following variables can be customized to fit your needs.

```javascript
{
  "compression_level": "7",
  "cpus": "1",
  "disk_size": "40000",
  "headless": "false",
  "memory": "512",
  "mirror": "http://releases.ubuntu.com",
  "token" : "{{env `ATLAS_TOKEN`}}",
  "chef_version": "12.11.18",
  "atlas_artifact": "pedrostanaka/cake-oven"
}
```

## WHY?

You may ask why create a new box for PHP development. Here are the answers:

1. I wanted to!
2. I wanted to learn Chef Provisioning + Vagrant + Packer
3. Did not find simple examples of how to build a VirtualBox box for Vagrant.
