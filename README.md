CoWFC for newer Ubuntu version
=
##### Front- and back -end website for the DWC network server emulator

# ⚠️ THIS PROJECT CAN HAVE PROBLEMS ⚠️
## This project are only for running on new version of Ubuntu not for having new update on the project, i don't have the skills for making security update on the project.

### ⚠️ PHP Error ⚠️
Following the updates of the repos it seems that the version of PHP used by the script is not installable any more.\
If you have a problem and managed to make the CoWFC server work with another version do not hesitate to make a pull request!

🔨 Contributing
-
Please open pull requests for the dev branch.\
I don't have time to take care of this fork anymore, it is not up to date compared to the initial version and will require some work to be updated following the removal of some features used by this fork which are not present on the original version.
I invite you first of all to participate in the development of the original project and secondly to try to update this version, I will accept with pleasure pull requests.

📝 How to use
-
First, you will need to be running on Ubuntu 14.04 or 16.04 or Debian 10. Otherwise the [setup script](https://github.com/FIREXDF/cowfc_installer) will not run.\
❌ Debian 10 : LAN Reported not working ! Only tested on a VPS using a domain name)

Please run the following command below to get started:
![image](https://upload.wikimedia.org/wikipedia/commons/thumb/9/9d/Ubuntu_logo.svg/100px-Ubuntu_logo.svg.png)

`mkdir /var/www ; cd /var/www && wget https://raw.githubusercontent.com/FIREXDF/cowfc_installer-New-Ubuntu/master/cowfc.sh && chmod +x cowfc.sh && ./cowfc.sh`

After system reboot : `cd /var/www && ./cowfc.sh`

![image](https://www.debian.org/logos/openlogo-nd-25.png) Debian
----

`wget https://raw.githubusercontent.com/FIREXDF/cowfc_installer-New-Ubuntu/master/cowfc.sh && chmod +x cowfc-debian.sh && ./cowfc-debian.sh`

## Features
- Stats page shows who is online by game/country
- Admin panel to manage bans, whitelists, and more
- Directly edit the dwc_network_server_emulator settings

🔧 Error reporting
-
Create a new issue and communicate all informations that you can.

📖 Notes
-------

This script comes in 3 phases for Ubuntu. Each phase involves a reboot
-	Add the PHP 7.1 repo
-	Continue CoWFC install
-	Reboot after CoWFC install

This script comes in 1 phases for Debian.
-	Install CoWFC & Reboot

Ubuntu script use PHP 7.1 & MySQL<br/>
Debian script use PHP 7.4 & MariaDB<br/>
This version of CoWFC is not compatible with the original dwc_network_server_emulator ! We are using my [own fork](https://github.com/EnergyCube/dwc_network_server_emulator) !

# Screenshots
#### Login Page
![image](https://user-images.githubusercontent.com/10158714/30234202-09416e82-94c9-11e7-94ac-8aa6e8bf550d.png)
#### Main Dashboard
![image](https://user-images.githubusercontent.com/10158714/30234212-212eadf2-94c9-11e7-8b01-24c10f67ce7a.png)
#### User List - contains all the info an admin would need to identify a player
![image](https://user-images.githubusercontent.com/10158714/30234228-3f4ed5b4-94c9-11e7-814c-26d892d29707.png)
#### dwc_network_server_emulator Settings
![image](https://i.ibb.co/WFGxYdZ/settings.png)
#### Console Manual Activation
![image](https://i.ibb.co/GJd485w/consoles-waiting.png)

### More screenshots coming soon as we get further with development.

📋 TODO
-
- Integrate moderator rank system
- Integrate moderator account management portal
  - Only accessible by highest ranked moderators
  - Modification of users of the same rank must be done through shell
- Add more settings
- Support more Systems or Ubuntu version
- More ideas I'm sure we haven't thought of yet :p
