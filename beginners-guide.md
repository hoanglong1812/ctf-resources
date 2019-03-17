# A beginner's guide to setting up for your first CTF

If this is your first CTF, welcome! 

Kali Linux is a common OS used for offensive security. Many people run it as a VM. 
To do this: download a VM program ([Virtualbox](https://www.virtualbox.org/) and [VMWare Player](https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html) are common), then get a [Kali image](https://www.offensive-security.com/kali-linux-vm-vmware-virtualbox-image-download/).
You can also install it as your base OS (not recommended).

After installing Kali, you will also have to set up Burp Suite if you're planning to do web challenges. Burp Suite captures IP packets such as HTTP requests. It is installed by default on Kali but you will still need to [set it up](https://portswigger.net/burp/documentation/desktop/tools/proxy/using).

If you are using Firefox, [turn off captive portal](https://support.mozilla.org/en-US/questions/1157121) to avoid generating garbage requests.

FoxyProxy can be used as a proxy switcher to turn the proxy on and off. It is available as a Firefox and Google extension.
