# Offensive Security Tools for Termux

No needs a Device ROOTED ;)

[![Powered by JFrog Bintray](./.github/static/powered-by-bintray.png)](https://bintray.com)
[![Codacy Badge](https://app.codacy.com/project/badge/Grade/12cdb5d6ed82487385bb69104be4f6ee)](https://app.codacy.com/gh/4k4xs4pH1r3/termux/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)

There are located packages which were requested, but not added to the
[main][termux-packages] Termux repository due to various reasons. Packages
available here may have lower quality, be unstable or not work at all.

## Pre-Requisite

Download [F-Droid](https://f-droid.org/F-Droid.apk) in your Android, open it, search termux and install it.

Free Storage Space = 33.37 GB

Now open Termux, each one of this 3 steps needs and independent session, for that just slide from left to rigth in termux for see the option. "New Session"


## 1. Prepare Termux
```ShellSession
pkg update -y && pkg upgrade -y && pkg install termux-tools
```
#
```ShellSession
termux-setup-storage
```
#
```ShellSession
termux-wake-lock && export PATH=/sbin:/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin && export PATH=$PATH:/usr/local/sbin:/usr/local/bin
```
#

## (Optional) Building packages manually

You can build all packages manually by using provided docker image. The only
requirements are Linux-based host with Docker installed.

a. Clone this repository:
	```ShellSession
	git clone https://github.com/termux/unstable-packages
	```

b. Enter build environment (will download docker image if necessary):
	```ShellSession
	cd ./unstable-packages
	./start-builder.sh
	```
	Command shown above will start builder for Android 7 (API level 24). If you
	need to build package for Android 5, use `./start-builder-legacy.sh`.

c. Choose package you want to build and run:
	```ShellSession
	./build-package.sh -a ${arch} ${package name}
	```
	Replace `${arch}` with target CPU architecture and `${package name}` with
	package name you want to build.

## Contributing

If you wish to contribute, please take a look on our [contributing guide](./CONTRIBUTING.md).

[termux-packages]: <https://github.com/termux/termux-packages>
#
#
#
#
#
## 2. Install Pre-Requisites:

```ShellSession
pkg update && pkg install unstable-repo root-repo x11-repo -y && apt update && apt install ruby neofetch coreutils busybox screenfetch vim nano python python-pip nodejs git openssh -y && screenfetch
```
#
```ShellSession
gem install nokogiri
```
#
```ShellSession
pkg update -y && pkg upgrade -y && pkg install python python2 ruby git php perl nmap bash clang nano figlet cowsay curl tar zip unzip tor tsu wget wcalc openssl bmon -y && pkg update -y && pkg upgrade -y && cp $(which pip) $PREFIX/bin/pip3 && neofetch && pkg install wget openssl-tool proot -y && neofetch
```
#

## 3.0 Install Kali Linux Nethuner (Method A)
```ShellSession
pkg install wget openssl-tool proot -y && hash -r && wget https://raw.githubusercontent.com/EXALAB/AnLinux-Resources/master/Scripts/Installer/Nethunter/nethunter.sh && bash nethunter.sh
```

## 3.1 Install Kali Linux NetHunter (Method B)

```ShellSession
termux-wake-lock;\
termux-setup-storage;\
apt-get update -y;\
apt-get install wget -y;\
wget https://raw.githubusercontent.com/Hax4us/Nethunter-In-Termux/master/kalinethunter;\
bash kalinethunter;\
rm *;\
startkali



apt-key adv --keyserver hkp://keys.gnupg.net --recv-keys 7D8D0BF6;\
wget https://http.kali.org/pool/main/k/kali-archive-keyring/kali-archive-keyring_2022.1_all.deb;\
apt --fix-broken install;\
dpkg -i ./kali-archive-keyring_2022.1_all.deb;\
rm kali-archive-keyring_2022.1_all.deb;\
apt-get update -y;\
apt-get install neofetch lolcat -y;\
echo "neofetch --logo | lolcat;neofetch model distro os kernel shell memory" >> ~/.bashrc;\
echo "PS1='
 ╭──────────[ $(whoami)@$(uname -n) ]─[ $PWD ]
 ╰── • '" >> /etc/bash.bashrc;exit



echo "clear;startkali;exit" >> ~/.bashrc;bash;exit
```
#
#
#
#
#

## 4. Install Nokogiri & Lolcat

From this point in advance execute in the same termux session
Only this lines as root
```ShellSession
apt update -y && apt install gem ruby -y
```

#
```ShellSession
gem install nokogiri
```

#
```ShellSession
gem install lolcat
```

## 5. Update System as root

```ShellSession
apt install neofetch -y && neofetch && gem install nokogiri && apt-get autoclean && apt install -f && apt -f install && apt autoremove -y && apt-get clean cache && apt update && apt-get autoclean && apt-get clean cache && apt update && apt update -y && apt full-upgrade -y --allow-downgrades && dpkg --configure -a && cd && neofetch
```

```ShellSession
apt update -y && apt install git -y && cd /usr/share && mv /usr/share/wordlists /usr/share/wordlists_bck && git clone https://github.com/4k4xs4pH1r3/SecLists.git /usr/share/wordlists && cd /usr/share/wordlists_bck/ && mv * -u -f /usr/share/wordlists/ && cd /usr/share/ && git clone https://github.com/danielmiessler/SecLists.git /usr/share/SecLists && cd && apt install neofetch screenfetch -y && neofetch && apt install nmap metasploit-framework asciinema steghide radare2 mtr firmware-realtek net-tools wpasupplicant wireless-tools -y && screenfetch && apt-get autoclean && apt install -f && apt -f install && apt autoremove -y && apt-get clean cache && apt update && apt-get autoclean && apt-get clean cache && apt update && apt update -y && apt full-upgrade -y --allow-downgrades && sudo dpkg --configure -a && cd && sudo apt-get install python python3 python-pip python3-pip python-dev python-setuptools -y && neofetch && bash <(wget -qO- https://git.io/vAtmB)
```

Close Termux and Open Again

## 6. Install Metasploit omnibus Nightly:
```ShellSession
    apt install nmap nginx -y && curl https://raw.githubusercontent.com/rapid7/metasploit-omnibus/master/config/templates/metasploit-framework-wrappers/msfupdate.erb > msfinstall && \
    chmod 755 msfinstall && \
    ./msfinstall
```
#
```ShellSession
gem install lolcat nokogiri bundle rails   
```
```ShellSession
gem update --system
```

#
    
## 7. Add Vuln + Vulners + Vulscan NSE as root

Specialized Scripts to get CVE's details with Nmap & Metasploit

```ShellSession
apt install git neofetch screenfetch -y && cd /usr/share/nmap/scripts && git clone https://github.com/scipag/vulscan && git clone https://github.com/vulnersCom/nmap-vulners.git && cd vulscan/utilities/updater/ && chmod +x updateFiles.sh && ./updateFiles.sh && neofetch && cd /opt/metasploit/common/share/nmap/scripts && git clone https://github.com/scipag/vulscan && git clone https://github.com/vulnersCom/nmap-vulners.git && cd /usr/share/nmap/scripts/vulscan/utilities/updater && chmod +x updateFiles.sh && ./updateFiles.sh && cd && screenfetch
```

```ShellSession    
sudo pip install --no-cache-dir -U crcmod
```
    
For display help for the individual scripts use this option
   
    --script-help=$scriptname
   
To get an easy list of the installed scripts, use 

    locate nse | grep nmap
#
#
The db_nmap sessions will be saved in xml for you can restart an early scan using
    
    msfconsole
    db_nmap --resume /root/.msf4/local/file.xml
    
The history of Metasploit commands are here:

    /root/.msf4/history
    
## 8. Start Metasploit

```ShellSession
apt-get autoclean && apt install -f && apt -f install && apt autoremove -y && apt-get clean cache && apt update && apt-get autoclean && apt-get clean cache && apt update && apt update -y && apt full-upgrade -y --allow-downgrades && dpkg --configure -a && cd && neofetch
```


Configure the services and database of Metasploit Framework 5:

    su 
    msfupdate
    update-rc.d postgresql enable && update-rc.d nginx enable && service postgresql start 
    su postgres
    createuser root -P
    createdb —owner=root msfdb
    exit
    
Close terminal
   
Open a new terminal as a normal user and verify that services are running and initiate the database of Metasploit Framework 5. 
  #   

```ShellSession
service --status-all
```

It's time to open Metasploit Framework 5 (Works in Kali Linux and Ubuntu Cosmic)

```ShellSession
neofetch && msfdb init && /opt/metasploit-framework/bin/./msfconsole
```

#
 (for repair use "msfdb reinit")

   

## Update and Check Metasploit Framework:

    msfupdate
    db_status
    db_rebuild_cache
    load nexpose
    load nessus
    save
#   
#
#
#
 

## 9. Create and Save your workspace

    workspace -a ad
    
    setg Prompt x(%whi%H/%grn%U/%whi%L%grn%D/%whi%T/%grn%W/%whiS%S/%grnJ%J)
    setg ConsoleLogging y
    setg LogLevel 5
    setg SessionLogging y
    setg TimestampOutput true
    save
    exit

Make a backup each time that you need of each one of your workspaces by separately

    db_export -f xml /root/msfuExported.xml

Importing a file from an earlier scan (This is done using db_import followed by the path to our file.)

    db_import /root/msfu/nmapScan
