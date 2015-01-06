bashii
======

A suckless tool reimplemented in bash


Getting started
---------------

- Clone this repo: `git clone https://github.com/izabera/bashii.git`
- Set your parameters in `~/.iirc` or export the following variables:  
  `export nick=mynick host=irc.my-host.net port=6667`
- Run it with `./bashii &`

`bashii` will now create a fifo and a log file for each channel/target.

You can start by joining a channel:  `echo '/j #channel' > fifo-my-host`  
Now everything you write in `fifo-my-channel` will be sent to that channel.

 
Visual improvements
-------------------

To make it a bit more comfortable, follow the tips at 
http://tools.suckless.org/ii/usage
(Note: any tool made for ii will need some minor tweaks for the channels.)

Even a simple `tmux` + `cat > fifo` + `tail -f` could be a good start.

Sample screenshot that shows how nice looking it is:
![screenshot](http://i.imgur.com/gzEZ3t6.png)


Other improvements
------------------

Found a bug?  Need an extra feature?  Just send a mail to izaberina AT google's
mail DOT com.  
Patches welcome!


License
-------

This is free software \o/  
Play with it, it's ISC licensed. 
