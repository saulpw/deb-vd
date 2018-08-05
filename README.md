# VisiData Debian Repository

deb-vd is a [Debian repository](https://wiki.debian.org/DebianRepository) for more convenient installation and updating of [VisiData](https://github.com/saulpw/visidata) on Linux distributions.

This repository contains VisiData v1.2.1.

If you are looking for installation instructions for VisiData on MacOS/X or using pip3, they are available [here](https://github.com/saulpw/visidata/blob/stable/README.md#installation).

Currently, VisiData v1.0 is in Debian unstable's [main repository](https://launchpad.net/ubuntu/+source/visidata) and is projected to be released on buster. Instructions for installing from Debian are [here](https://github.com/saulpw/visidata#install-via-apt).

## Install

Grab our public key
```
wget http://visidata.org/devotees.gpg.key
apt-key add devotees.gpg.key
```

Add our repository to apt's search list
```
sudo apt-get install apt-transport-https
sudo vim /etc/apt/sources.list
    deb [arch=amd64] https://raw.githubusercontent.com/saulpw/deb-vd/master sid main
sudo apt-get update
```
You can then install VisiData by typing:
```
sudo apt-get install visidata
```

VisiData can then be updated with every subsequent release using:
```
sudo apt-get update
sudo apt-get install visidata
```

## About
VisiData was created and is being developed by [Saul Pwanson](http://saul.pw) &lt;saul@visidata.org&gt;. The debian package and repository is being maintained by [Anja Kefala](https://github.com/anjakefala) &lt;anja@visidata.org&gt;.
