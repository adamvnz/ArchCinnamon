# Installing Cinnamon on Arch Linux

This is my configuration for Cinnamon to be used on Arch Linux.

In the installation folder is all the data, explanations and scripts for you to have a great working environment.

Before I installed xorg and all its packages. Then you install cinnamon. See wiki of Arch Linux.

	sudo pacman -S cinnamon

I installed the mdm-display-manager already and enabled it.

	packer mdm-display-manager
	sudo systemctl enable mdm
	sudo systemclt start mdm



![Screenshots](http://erikdubois.be/wp-content/uploads/2015/05/archcinnamon12.jpg)





# A R C H L I N U X 
----------------------- 

I started using Archlinux as a learning experience. I have tried installing all kinds of desktop environments (DE) and formatted many times my ssd's to start from scratch. After a while it was more practical to have a script of some kind to record the knowledge and to automate the things I had already learned. They became repetitive in nature.

The goal is to be quickly up and running after a clean install. 

That's why I have written a script to do just that. 

#1. Installation of the base system

I started following the guide of 

https://wiki.archlinux.org/index.php/Beginners%27_guide

After this base installation you will end up in a black screen (terminal) with no graphical environment what so ever. Then it is up to the user to install xorg and choose a Desktop Environment.

Good options are

	- xfce
	- gnome
	- kde
	- openbox
	- i3

We will install CINNAMON this time.

	sudo pacman -S cinnamon

https://wiki.archlinux.org/index.php/Cinnamon




![Screenshots](http://erikdubois.be/wp-content/uploads/2015/05/archcinnamon3.jpg)




#2. Installation of the software

At this point you have a working cinnamon with a mdm display manager.

Then I run an installation script to quickly  get all my software. For me this was quite a learning process, since I was a Redhat, Ubuntu, Linux Mint kind of guy over the last two decades. 

The idea is to download (if you have internet connection) the github files :

	sudo pacman -S git    (if needed - normally present)

	git clone https://github.com/erikdubois/ArchCinnamon.git



Then you can start running the underneath mentioned script to be found in the folder "installation".

	step_1_install_cinnamon_software_vx.sh

I am using zsh because of the great number of awesome themes and plugins. Remember that you need to type this line after the script.
Quit the terminal and restart it again via CTRL+ALT+T.

	sudo chsh username -s /bin/sh

Then I opt to use the network-manager so the icon in the systembar (right-bottom) works.

	step_2_back_online_vx.sh

If you like you can get some awesome themes and icons with 

	step_ 3_theming_vx.sh

A specific script for samba (sharing of maps on your home network) if you need it.



![Screenshots](http://erikdubois.be/wp-content/uploads/2015/05/archcinnamon21.jpg)



Now it is up to you to change the settings of cinnamon.

Checkout system settings (effects, themes, window tiling and edge flip, ...)


Then you take the script apart and write your own code.

------------------------------------
#But that is the fun in Linux.

You can do whatever <b>Y O U</b> want.

Be free and share the knowledge.
------------------------------------



![Screenshots](http://erikdubois.be/wp-content/uploads/2015/05/archcinnamon4.jpg)