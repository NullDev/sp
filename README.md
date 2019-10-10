# sp
Debian/Ubuntu Package for sp - a command-line client for Spotify's dbus interface

> _sp is a command-line client for Spotify's dbus interface. Play, pause, skip and search tracks from the comfort of your command line._


Original Script by Wander Nauta: <br>
https://gist.github.com/wandernauta/6800547

## How to install: 

- [Download](https://github.com/NLDev/sp/archive/master.zip) the repository and exctract it.
- Open a terminal and navigate into the newly extracted folder.
- Finally run: <br>
  $ `sudo dpkg -i sp_1.0-1_all.deb`
- (Optional) Delete the `.deb` file, it's containing folder and the archive file.
- Done.

<hr>

## (Optional) Building the `.deb` yourself:

- Install the required packages: <br>
  $ `sudo apt-get install -y dh-make devscripts`
- Clone the repository and navigate into it: <br>
  $ `git clone https://github.com/NLDev/sp.git && cd sp`
- Remove the existing `.dep`: <br>
  $ `rm sp_1.0-1_all.deb`
- Navigate into the [sp-1.0](https://github.com/NLDev/sp/tree/master/sp-1.0) folder: <br>
  $ `cd sp-1.0`
- Use the following command to build the .dep: <br>
  $ `debuild -us -uc`
- Now navigate back into the repository root and you should see your `.dep`: <br>
  $ `cd .. && ls`
- Finally, install it: <br>
  $ `sudo dpkg -i sp_1.0-1_all.deb`
- Done.

<hr>
