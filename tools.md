# CTF tools
Highly, *highly* recommend creating a "tools" directory/folder and installing some of these.

#### A quick note on Git
Git is a version control framework. In the context of tooling, it allows you to copy someone else's tool from sites like Github and update it when they update their source code.

#### Python
I've included a number of Python packages on this list because I use Python scripting a lot when CTFing. Where a command reads `pip3`, you may just need to just use `pip`, depending on your platform and your Python install.

## Crypto
[RsaCtfTool](https://github.com/Ganapati/RsaCtfTool): Great for cracking weak RSA keys. 
Clone it from github. (Note: one of the prerequisites is the python gmpy2 package. Use `apt-get install python3-gmpy2` to get gmpy2 - using `pip install` will get you a non-working package.)

[CyberChef](https://gchq.github.io/CyberChef/): Describes itself as the Cyber Swiss Army Knife and honestly, it kind of is. Does all sorts of format conversions and breaks simple ciphers. 
Have a funky looking string in a crypto or misc challenge? Throw it in CyberChef. 
Hosted online, but you can also download a copy to run in your browser offline.

## Reversing
Binary Ninja

[radare2](https://github.com/radare/radare2): I have no idea how to use this but it's free and I'm told it's great.

Ghidra

[Peda](https://github.com/longld/peda): An add-on to gdb, a debugger.
A quick, practical intro to using GDB-Peda can be [found here](https://www.blackroomsec.com/reversing-small-crackme-w-gdb-peda/).
Clone it from github (see instructions in the README in the installation section.)

## Pwn
[pwntools](https://github.com/Gallopsled/pwntools): A Python package for pwn challenges. Only available for Python 2.7. Get it with `pip install pwntools`. 

## Forensics
[scapy](https://scapy.readthedocs.io/en/latest/): A Python package that reads pcap files. Use Wireshark for the GUI, but scapy rules if you want to script with the packet captures. 
Get it with `pip3 install scapy`.


## Web
[requests](http://docs.python-requests.org/en/master/): A Python package that does http requests. Get it with `pip3 install requests`.



## Miscellaneous
steghide