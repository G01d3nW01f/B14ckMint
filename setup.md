# B14ckMint is my setup of LinuxMint For Hacking

# 1 Download ISO image

![image](https://user-images.githubusercontent.com/75846902/154009279-a9dc595e-b8b9-4b36-b93a-4b8f2f138fe3.png)

https://linuxmint.com/download.php


 Download the iso file for install.

You can chose any versions of desktop systems
Bur My recommend is Xfce, because Light and fast

# 2 Make the Bootable USB 

![image](https://user-images.githubusercontent.com/75846902/154009826-bcf731d1-7d9e-4e28-859a-ec9de43441b9.png)

https://rufus.ie/en/

rufus is bootable USB maker for windows.
This program is so useful and safe.........probably

refference to below link <Japanese>

https://linuxfan.info/make-linux-install-usb-on-windows

# 3 Boot On 
 
put the USB card to machines port,
power on and after the press the F2 key or Delete key

![image](https://user-images.githubusercontent.com/75846902/154010774-22b0c241-88a0-45fb-a0bb-2230ab7abe9b.png)

[Start LinuxMint]
 
 
# 4 Update
 
```
 sudo apt update
 sudo apt upgrade
```
 
# 5 Install the tools
 
```
 sudo apt install git
 sudo apt install python3-pip 
 sudo apt install nmap
 sudo apt install sqlmap
 sudo apt install hashcat
```
 
# 6 Install WPscan
 ![image](https://user-images.githubusercontent.com/75846902/154011661-173b9248-1c44-4db5-8a44-961623c6f7b9.png)

```
sudo apt install ruby

sudo apt install build-essential libcurl4-openssl-dev libxml2 libxml2-dev libxslt1-dev ruby-dev  libgmp-dev zlib1g-dev

sudo gem install wpscan 
```
 
# 7 Install John

![image](https://user-images.githubusercontent.com/75846902/154012238-40e79cf6-a93d-46a3-84a7-afb9f332bb79.png)
 
 ```
 sudo apt-get install build-essential libssl-dev
  
  sudo apt-get install yasm libgmp-dev libpcap-dev libnss3-dev libkrb5-dev pkg-config libbz2-dev zlib1g-dev
  
  cd ~/src
  
  git clone git://github.com/magnumripper/JohnTheRipper -b bleeding-jumbo john
  
  cd ~/src/john/src
  
  ./configure && make -s clean && make -sj4
  
  ../run/john --test
 ```

# 8 Install Metasploit
 
 ![image](https://user-images.githubusercontent.com/75846902/154012579-b9a31050-c973-42ce-b516-906b73acf684.png)

 
 ```
 curl https://raw.githubusercontent.com/rapid7/metasploit-omnibus/master/config/templates/metasploit-framework-wrappers/msfupdate.erb > msfinstall && \
  chmod 755 msfinstall && \
  ./msfinstall
 ```
 
# 9 Install searchsploit
 
 ![image](https://user-images.githubusercontent.com/75846902/154013242-7a6e4f7f-e0ed-40d7-9a0f-4c398dca9f2b.png)

 
 ```
 git clone https://github.com/offensive-security/exploitdb.git /opt/exploit-database
 
 ln -sf /opt/exploit-database/searchsploit /usr/local/bin/searchsploit
 
 cp -n /opt/exploit-database/.searchsploit_rc ~/
 
 vim ~/.searchsploit_rc
 ```
 
 
