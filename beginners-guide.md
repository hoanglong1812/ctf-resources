# A beginner's guide to setting up for your first CTF


## Set up your computer
Conventional wisdom says to set up a virtual machine on your computer. You could also boot off a USB, but it's more difficult. You could even install it as your base OS but that is really, really, *really* **not** recommended.

### Virtual Machines 101
Virtual machines (VMs) are like computers that run on your computer. They're helpful to us because it allows separation between the computer that you use for personal stuff and the computer where you install all of your hacking tools.

In VM talk, the OS that your computer is running normally is the "host" and the OS that runs on top of it is called the "guest".

### Installing Kali Linux
A really popular way to CTF is using Kali Linux in a VM. To do this: download a VM program ([Virtualbox](https://www.virtualbox.org/) and [VMWare Player](https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html) are popular), then download a [Kali image](https://www.offensive-security.com/kali-linux-vm-vmware-virtualbox-image-download/). 
You'll want to get the one that works for the VM program - the .iso files may be difficult to set up.

### Using your host machine 
You can use your host machine for some things, even though it's not recommended. 

You may want to install [Burp Suite](https://portswigger.net/burp/communitydownload) (see below for more setup instructions), but in that case make sure that the browser that you install the certificate on is not used for any other purpose - the certificate would allow Burp to identify any site for you.

Other tools to consider for your host are:
+ a Python IDE for scripting (I use [PyCharm](https://www.jetbrains.com/pycharm/) and [VS Code](https://code.visualstudio.com/)) and, if on Windows, [Git](https://www.atlassian.com/git/tutorials/install-git) (should be installed be default for Mac and Linux)
+ a Bash shell (e.g. [Bash on Ubuntu on Windows](https://docs.microsoft.com/en-us/windows/wsl/install-win10) or the Git Bash shell (included with Git for Windows) for Windows, terminal comes installed with Mac and Linux)
+ a hex editor (I like [HxD](https://mh-nexus.de/en/downloads.php) on Windows)
+ an unzipping utility (e.g. [7Zip](https://www.7-zip.org/download.html))
+ a nice text editor (e.g. [Atom](https://atom.io/) or [Notepad++](https://notepad-plus-plus.org/))
+ a network protocol analyser ([Wireshark](https://www.wireshark.org/))

Chat clients like Slack and Discord can be handy for both intro flags and getting hints.

## Setting up basic tools

### Browser things
I would highly recommend using Firefox and FoxyProxy with Burp to do web app challenges.

Burp Suite is installed by default on Kali Linux, but you will need to [set it up](https://support.portswigger.net/customer/portal/articles/1783087-installing-burp-s-ca-certificate-in-firefox) by adding the CA cert to your browser. 

If you are using Firefox, [turn off captive portal](https://support.mozilla.org/en-US/questions/1157121) to avoid generating garbage requests.

FoxyProxy can be used as a proxy switcher to turn the proxy on and off. It is available as a [Firefox add-on](https://addons.mozilla.org/en-US/firefox/addon/foxyproxy-standard/) and Google extension.
Once installed, you need to add Burp by selecting "Add", then filling in the details as follows:
+ Name: Burp (or another name of your choice)
+ IP address: 127.0.0.1
+ Port: 8080

Then click "Save". Turn the proxy on by right-clicking on the little fox icon next to the URL bar and selecting "Use Burp for all URLs". 


