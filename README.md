# JuiceShopped

Unofficial VirtualBox virtual machine instance of OWASP Juice Shop

### Contributors: [Aut0exec](https://aut0exec.blogspot.com)

## Features
	- Devuan Daedalus instance
	- Pre-installed and configured to auto start on boot
		- OWASP Juice Shop version 15.0.1 Node 18
		- VAmPI - Vulnerable API

## Relevant Information

While there shouldn't be a need to log in to the console, should one need to, the information is as follows:

Low privilege user  - __user__:__Password123__

Root privilege user - __root__:__juiceisworththesqueeze__

## Installation

__WARNING!__ Juice Shop is designed to be vulnerable. __DO NOT__ connect this VM to the Internet or sensitive networks.

1. Download the OVA from the [releases page](https://github.com/aut0exec/JuiceShopped/releases)
1. Launch virtualbox
1. File -> Import Appliance
1. Under the source section, select Local File System and then navigate to the location where the OVA file was downloaded
1. The default settings should be sufficient on the right side of the import window
1. Click Import in the bottom right to import the appliance
1. Once the import finishes, start Juice Shop. The machine expects a DHCP server to be present and will automatically request an address.
	- VirtualBox will automatically configure port forwards from the host to the guest for ports TCP/3000 and TCP/5000. Any scanning or interaction from the host with the virtual machine can be done via 127.0.0.1:3000 or 127.0.0.1:5000.

## Credits/Thanks
[Erev0s VAmPI](https://github.com/erev0s/VAmPI)

+ Thanks for the vulnerable API to add to this project!

[OWASP Foundation](https://owasp.org/www-project-juice-shop/)

+ Thanks for maintaining, releasing, and developing Juice Shop and a number of amazing other projects!

[Oracle](https://www.virtualbox.org/)

+ Thanks for creating, maintaining, and providing the virtualbox hypervisor!

[Devuan](https://www.devuan.org/)

+ Keep up the great work on such an awesome fork of Debian!
