# OpenWrt builder

For OpenWrt >= 21.02

## Install dependencies

```
sudo apt-get install git git-core curl rsync
sudo apt-get install build-essential gawk gcc-multilib flex git gettext libncurses5-dev libssl-dev
sudo apt-get install python3-distutils rsync unzip zlib1g-dev
```

## Build firmware

```
git clone https://github.com/JekisV/builder -b v25 openwrt-v25
cd openwrt-v25

./xcreate.sh -v xq-25.12.6
cd xq-25.12.6

./xupdate.sh -f

./xmake.sh -f -t r3d
```
