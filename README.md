# Install latest YARA version from source code in Kali Linux.

>apt-get updates.  
>tar -zxf [version].tar.gz
## Install the depencies first : automate, libtool, make, gcc, libssl-dev and libmagic-dev
sudo apt-get install automake libtool make gcc pkg-config autoconf libssl-dev libmagic-dev

### Install Yara
* cd yara-[version]
* ./bootstrap.sh
* ./configure --with-crypto --enable-magic
* make 
* sudo make install

##### Update Shared Libraries
sudo ldconfig

