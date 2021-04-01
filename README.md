# Install latest YARA version from source code in Kali Linux.
> Download latest release [yara.yar](https://github.com/VirusTotal/yara/releases/tag/v4.1.0-rc2)  
> apt-get updates.  
>tar -zxf [version].tar.gz
## Install Yara dependencies
sudo apt-get install automake libtool make gcc pkg-config autoconf libssl-dev libmagic-dev

### Install Yara
* cd yara-[version]
* ./bootstrap.sh
* ./configure --with-crypto --enable-magic
* make 
* sudo make install

### Update Shared Libraries
sudo ldconfig

