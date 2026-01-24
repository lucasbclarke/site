### Pihole Server

I'd had an old Dell laptop from the Windows 7 era, sitting unused in a cupboard for a number of months. I occasionally pulled it out to install a new linux distribution that I had seen
but I didn't have any day to day use for the machine. I had heard of Pi-hole a number of months ago, and had mostly forgot about it until seeing it again online used in a home-lab
setup. Firstly, I installed Ubuntu Ubuntu 24.04.3 LTS as the base linux operating system, that Pi-hole would run off of. Next I simply went to the Pi-hole doccumentation and ran the curl command to pull down and then run the install script.
As the install script ran I was presented with a number of options in the TUI interface in regards to DNS and security. I decided to stay with the defaults as I did not have any reason
to change them. 

However while in the TUI setup I realised that I had not yet created a static IP address for this machine, which was required for Pi-hole to work correctly. So I exited the setup script
and went into my local router settings, where I set a static IP address for the dell laptop. Going back the machine I was now able to verify that the machine had recieved its static
address and so I restarted the Pi-hole setup again. After finishing the setup I navigated to the Pi-hole web interface using the static IP I had just set, with the suffix /admin.
On the web interface I was able to view all connected clients to the network and monitor which requests were denied and what addresses they corresponded too.

This setup worked quite well for the first few weeks, however I had been noticing that not all advertisments had been blocked. I knew that Pi-hole worked based on a list-based system
and that there was other lists that could potentially produce greater results. Subsequently I searched and found two more lists that at least claimed they worked well for moderate
add-blocking cases, which was all I needed. I then was able to simply copy the links to these lists, into the lists section of the Pi-hole web interface and restart the Pi-hole service.

After adding the extra lists the Pi-hole server had been running well for a number of weeks, up until a few days ago where I had started to notice a significant increase in the amount
of advertisments that I was seeing. As I had not been actively monitoring the Pi-hole web interface, I decided that would be the first place I should look. Howver when I attempted to 
navigate to the web interface I was met with a page not found screen. As I was sure that the address was correct I decided to open the machine itself to see if there was an error that
had been reported. It turned out that there was a connection error which just required the Pi-hole service to be restarted and updated, and after doing so worked correctly as it had before.

Originally when starting this project I was concerned that all of the traffic on my network would be slowed down, as a result of running through my Pi-hole service. It turned out
however that this was not the case, and I have seen no noticeable drop in network performance, from any device connected to the network. And despite the machine being at least 16 years
old, it has been able to keep up with the traffic of my home network.

14.12.25 - 09:00 AM AEST
