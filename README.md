# Ros-inistall-steps
Ros install steps:
1. Download VirtualBox 6.1.34.
2. After download virtualBox 6.1.34 we leave and then download ubuntu 20.04.4 64bit.
3. We open VirtualBox then press new, and then fill in the following data. 
4. and then next and the memory size:1000MB then create a virtual hard disk now and the size is the limit on the amount of file data that a virtual machine will be able to store on the hard disk 20GB and then create.
5. Finally, the main interface of the program, virtual box, will appear finally, the main interface of the program, virtual box will appear, then we will click on setting to set up the ubuntu file in Ros and choose storage, then from the CD tab, choose the ubuntu 20.04.4 file, then save.
6. We return to the main page of the interface of the virtual box program and press start, then choose install ubuntu and complete the rest of the steps by pressing continue, then we fill in the following data: My Name and Password.
7. After that, we open a terminal to write the commands to download Rose in Ubuntu.

# Configure your Ubuntu respositories

echo "deb http://packages.ros.org/ros/ubuntu focal main" | sudo tee /etc/apt/sources.list.d/ros-focal.list

Set up your keys

sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

curl -sSL 'http://keyserver.ubuntu.com/pks/lookup?op=get&search=0xC1CF6E31E6BADE8868B172B4F42ED6FBAB17C654' | sudo apt-key add -

# Installation

sudo apt update

Desktop-Full Install:

sudo apt install ros-noetic-desktop-full

# Environment setup

source /opt/ros/noetic/setup.bash

echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc

Rose was downloaded successfully. 
To make sure, we type the command:

roscore
