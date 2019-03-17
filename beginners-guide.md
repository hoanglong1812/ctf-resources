# A beginner's guide to setting up for your first CTF

The text of this guide is in the context of CTFs but could also be applied to other applications.


## Set up your computer
Conventional wisdom says to set up a virtual machine on your computer. You could also boot off a USB, but it's more difficult.

### Virtual Machines 101
Virtual machines (VMs) are like computers that run on your computer. They're helpful to us because it allows separation between the computer that you use for personal stuff and the computer where you install all of your hacking tools.

In VM talk, the OS that your computer is running normally is the "host" and the OS that runs on top of it is called the "guest".

### Installing Kali Linux
A really popular OS for CTFing is Kali Linux. To run it, you'll need a virtual machine software and a Kali image.




### Using your host machine 
You can use your host machine, even though it's not recommended. 

You may want to install Burp (see below), but in that case make sure that the browser that you install the certificate on is not used for any other purpose - the certificate would allow Burp to identify any site for you.

Other tools to consider for your host are:
+ a Python IDE (I use PyCharm and VS Code) and, if on Windows, Git
+ a Bash shell (e.g. terminal for Mac and Bash on Ubuntu on Windows for Windows)
+ a hex editor (I like HxD)
+ an unzipping utility (like 7Zip)
+ a nice text editor (e.g. Atom or Notepad++)
+ a network protocol analyser (Wireshark)

Chat clients like Slack and Discord can be handy for both intro flags and getting hints.

## Setting up basic tools

### Browser things
I would highly recommend using Firefox and FoxyProxy with Burp to do web app challenges.

