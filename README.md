# JuiceShopped

Unofficial VirtualBox virtual machine instance of OWASP Juice Shop

### Contributors: [Aut0exec](https://aut0exec.blogspot.com)

## Features
	- Devuan Daedalus instance
	- OWASP Juice Shop version 14.1.1 Node 16
	- Pre-installed and configured to auto start on boot

## Relevant Information

While there shouldn't be a need to log in, should one need to, the information is as follows:

Low privilege user  - __user__:__Password123__

Root privilege user - __root__:__juiceisworththesqueeze__

## Installation

__WARNING!__ Juice Shop is designed to be vulnerable. __DO NOT__ connect this VM to the Internet or sensitive networks.

1. Download the OVA
1. Launch virtualbox
1. File -> Import Appliance
1. Under the source section, select Local File System and then navigate to the location where the OVA file was downloaded
1. The default settings should be sufficient on the right side of the import window
1. Click Import in the bottom right to import the appliance
1. Once the import has completed, got to the network settings and select the proper network configuration. __Host-only Adapter is STRONGLY encouraged.__
1. Once the proper network has been chosen, start Juice Shop. The machine expects a DHCP server to be present and will automatically request an address.
	- To deteremine address scope, check the network settings in VirtualBox's Host Network Manager or respective network configuration from above. Often nmap will make determining the address assigned to Juice Shop easier.

## Credits/Thanks
[OWASP Foundation](https://owasp.org/www-project-juice-shop/)

+ Thanks for maintaining, releasing, and developing Juice Shop and a number of amazing other projects!

[Oracle](https://www.virtualbox.org/)

+ Thanks for creating, maintaining, and providing the virtualbox hypervisor!

[Devuan](https://www.devuan.org/)

+ Keep up the great work on such an awesome fork of Debian!
