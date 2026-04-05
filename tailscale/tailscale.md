### Tailscale

Tailscale is a free, zero-config mesh VPN service which is built on the WireGuard protocal. It allows for secure peer-to-peer connection accessible to users of various technical
abilities. A wide variety of systems are supported including, Windows, Mac, and Linux desktops, Andriod and IOS phones, and other IOT devices such as rasberry pi's and Network Attached
Storage devices.

The connection between devices in the "Tailnet" is mainted regardless of physical location, so from your laptop in a coffee shop, you could access your home media server, without
the need to configure port forwarding or other firewall options. You can also connect to other devices on your home network, regardless if they are connected to tailscale or not,
through a subnet router.

For me, I wanted to be able to access my home network storage, and SSH into my home systems, from any location. I am able to achieve both of these goals through tailscale with very
little difficulty. The only setup required was the installation of tailscale on my devices, logging into the admin interface using github (this can also be achived through microsoft,
apple and google), and configuring one of my devices (the Dell laptop running Pihole) as a subnet router.

There are a variety of other features offered by Tailscale which I have yet to use, such as Aperture to manage AI models and the exit nodes feature.

5.4.26 - 07:16 PM AEST
