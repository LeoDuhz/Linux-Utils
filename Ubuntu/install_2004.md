## 1 change source
cd /etc/apt

sudo cp sources.list sources.list.copy

sudo gedit sources.list

change to sources like tsinghua source...

https://mirror.tuna.tsinghua.edu.cn/help/ubuntu/

sudo apt-get update

## 2 install NVIDIA drivers
https://blog.csdn.net/weixin_44599715/article/details/124366114 

blacklist nouveau driver

sudo gedit /etc/modprobe.d/blacklist.conf

blacklist nouveau

options nouveau modeset=0

sudo reboot

install either from Software&Update or NVIDIA official drivers

## 3. remove something you don't want
e.g.:
sudo apt-get --purge remove gnome-mines

## 4. change input method
sudo apt-get install fcitx-googlepinyin

https://www.cnblogs.com/yibeimingyue/p/15591832.html 

https://shurufa.sogou.com/linux/guide

## 5. install chrome
https://www.google.cn/intl/zh-CN/chrome/

## 6. other Apps
VSCode https://code.visualstudio.com/docs/?dv=linux64_deb 

WPS https://linux.wps.cn/ 

Miniconda https://docs.conda.io/en/latest/miniconda.html 

Foxit PDF READER https://www.foxit.com/pdf-reader/ 

Typora https://zahui.fan/posts/64b52e0d/

Albert https://albertlauncher.github.io/installing/

imwheel https://blog.csdn.net/a244068468/article/details/88364226

Anydesk https://anydesk.com/en

Baidu Netdisk https://pan.baidu.com/download?from=header#linux

Brightness Controller https://blog.csdn.net/weixin_44120025/article/details/118875998

Sublime Merge


## 7. apt install
sudo apt install vim git gcc python3-pip cmake curl

## 8. install ClashX
https://glados.rocks/console/clash

## 9. setup Git for Github

ssh-keygen -o -t rsa -C "github@mcnz.com"

copy id_rsa.pub into github sshkey setting

## 10. install Zotero
download from https://www.zotero.org/start 

sudo mv Zotero_linux-x86_64 /opt/zotero/

cd /opt/zotero

sudo chmod +x zotero

sudo chmod +x zotero-bin

sudo ./set_launcher_icon

ln -s /opt/zotero/zotero.desktop ~/.local/share/applications/zotero.desktop

reference: https://blog.csdn.net/xinjieyuan/article/details/105407564 & https://blog.csdn.net/aiboom/article/details/123245533 

then set up the webdev for sychronization

## 11. ROS

git clone git@github.com:LeoDuhz/Linux-Utils.git

cd Linux-Utils/ros

chomd +x install-ros-noetic.bash

./install-ros-noetic.bash
