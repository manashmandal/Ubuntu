# Ubuntu
### Solutions of some problems
####### DPKG

`Link: http://ubuntuforums.org/showthread.php?t=1894744`

>sudo -s

>cd /var/cache/debconf

>rm *.dat

>apt-get update && apt-get upgrade


###### #Bruteforce lock problem solved

`Link: http://unix.stackexchange.com/questions/147928/i-cant-install-new-packages-and-cant-update-and-upgrade`

> fuser /var/lib/dpkg/lock /var/lib/apt/lists/lock

> ls -l /var/lib/dpkg/lock /var/lib/apt/lists/lock 

> fuser -k /var/lib/dpkg/lock /var/lib/apt/lists/lock
