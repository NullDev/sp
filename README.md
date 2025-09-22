# sp
Debian/Ubuntu Package for sp - a command-line client for Spotify's dbus interface

> _sp is a command-line client for Spotify's dbus interface. Play, pause, skip and search tracks from the comfort of your command line._


Original Script by Wander Nauta: <br>
https://gist.github.com/wandernauta/6800547

Find it on Launchpad: https://launchpad.net/sp

## How to install: 

- [Download](https://github.com/NullDev/sp/releases/download/1.0/sp_1.0-1_all.deb) the binary.
- Open a terminal and navigate into the folder containing the downloaded binary.
- Finally run: <br>
  $ `sudo dpkg -i sp_1.0-1_all.deb`
- (Optional) Delete the `.deb` file, it's not needed anymore.
- Done.

<hr>

## (Optional) Building the `.deb` yourself:

- Install the required packages: <br>
  $ `sudo apt-get install -y dh-make devscripts`
- Clone the repository and navigate into it: <br>
  $ `git clone https://github.com/NullDev/sp.git && cd sp`
- Remove the existing `.deb`: <br>
  $ `rm sp_1.0-1_all.deb`
- Navigate into the [sp-1.0](https://github.com/NullDev/sp/tree/master/sp-1.0) folder: <br>
  $ `cd sp-1.0`
- Use the following command to build the .deb: <br>
  $ `debuild -us -uc`
- Now navigate back into the repository root and you should see your `.deb`: <br>
  $ `cd .. && ls`
- Finally, install it: <br>
  $ `sudo dpkg -i sp_1.0-1_all.deb`
- Done.

<hr>
