# Mystic v1.2 (update July, 2021)

Site : http://mysticpool.tk

Official Yiimp (used in this script for Yiimp Installation): https://github.com/tpruvot/yiimp
Original Yiimp Installer : https://github.com/cryptopool-builders/multipool_original_yiimp_installer


***********************************

## Use Ubuntu Server 16.04 / 18.04

Only use this scrypt on a fresh install

- sudo apt update
- sudo apt upgrade
- reboot 
- sudo -i (Gives root)
- adduser pooladmin (pooladmin is an example...)
- adduser pooladmin sudo
- su - pooladmin
- exit
- su - pooladmin
- sudo apt -y install git
- git clone https://github.com/StaticM223/Mystic_Pool_Scrypt.git
- cd yiimp_install_scrypt/
- bash install.sh (Do NOT use sudo or root)
- sudo apt install php7.3-memcache php7.3-memcached memcached
- Reboot after everything is installed

Finish !
- Go http://xxx.xxx.xxx.xxx or https://xxx.xxx.xxx.xxx (if you have chosen LetsEncrypt SSL)
- Go http://xxx.xxx.xxx.xxx/site/myadmin or https://xxx.xxx.xxx.xxx/site/myadmin to access Panel Admin

###### :bangbang: **YOU MUST UPDATE THE FOLLOWING FILES :**
- **/var/web/serverconfig.php :** update this file to include your public ip (line = YAAMP_ADMIN_IP) to access the admin panel (Put your PERSONNAL IP). update with public keys from exchanges. update with other information specific to your server..
- **/etc/yiimp/keys.php :** update with secrect keys from the exchanges (not mandatory)


###### :bangbang: **IMPORTANT** : 

- The configuration of yiimp and coin require a minimum of knowledge in linux
- Your mysql information (login/Password) is saved in **~/.my.cnf**

***********************************

If this helped please donate
- LTC Donation : LYhupoDpFHF69dc9KSAdRpTPhVM6aHajF5
- BTC Donation : bc1q6m3nzahxf8d26tcx0ct42lesq9h0x7pcv2zfr6
- ETH Donation : 0xd7779610e01c556efa4004320Aa1E60844998434
