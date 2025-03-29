# Kali Linux for Termux V2

![Kali Linux](https://i.imgur.com/hppysI0.png)

This script installs a lightweight Kali Linux environment in Termux with enhanced features for ethical hacking, penetration testing, and security research.

## Features
- Full Kali Linux environment in Termux
- Regular updates with the latest security patches
- Optimized for mobile performance and low resource consumption
- Pre-installed ethical hacking and penetration testing tools
- Easy start and stop scripts
- Automatic package updates and dependency management
- Multi-user support
- VNC support for graphical interface
- Secure access with SSH support
- Advanced networking tools
- Customizable configurations for advanced users
- Supports Metasploit, Nmap, SQLmap, and more
- Ability to install additional tools from Kali repositories
- Tor and ProxyChains support for anonymous browsing
- Encrypted file system support for secure data storage

## Installation

Make sure you have Termux installed. Then, run the following commands:

```sh
pkg update && pkg upgrade -y
pkg install git -y
git clone https://github.com/sathanicc/KALI-LINIX-FOR-TERMUX-V2.git
cd KALI-LINIX-FOR-TERMUX-V2
bash install.sh
```

## Usage

After installation, start Kali Linux with:

```sh
./start-kali.sh
```

To stop the Kali Linux session, use:

```sh
exit
```

## Additional Features

### Graphical Mode (VNC)
Run Kali Linux with a desktop environment:
```sh
./start-vnc.sh
```

### Update & Upgrade Packages
Ensure your system is up to date:
```sh
apt update && apt upgrade -y
```

### Pre-installed Tools
- **Networking & Scanning:** Nmap, Wireshark, Netcat, Bettercap
- **Exploitation:** Metasploit Framework, Hydra, SQLmap, Routersploit
- **Wireless Attacks:** Aircrack-ng, Wifite, Kismet
- **Password Cracking:** John the Ripper, Hashcat, Crunch
- **Forensics & Reverse Engineering:** Binwalk, Radare2, Volatility
- **Web Application Testing:** Burp Suite, Nikto, Wpscan
- **Social Engineering Tools:** SET, SocialFish, Zphisher
- **Anonymous Browsing:** Tor, ProxyChains, Anonsurf
- **File Encryption & Security:** VeraCrypt, GPG, EncFS

### Secure Access
Enable SSH for secure remote access:
```sh
apt install openssh -y
sshd
```

### Customization
Modify the Kali environment to suit your needs by editing configuration files and installing additional tools:
```sh
nano ~/.bashrc
```

### Tor & ProxyChains Support
Enable anonymous browsing and penetration testing with Tor:
```sh
apt install tor proxychains -y
tor &
proxychains nmap -sT example.com
```

### Encrypted Storage
Secure your sensitive data using encrypted file systems:
```sh
apt install veracrypt -y
veracrypt -c
```

## Notes
- This script requires an active internet connection.
- Some tools may require root access for full functionality.
- Ensure your device has sufficient storage before installation.
- Using hacking tools without permission is illegal; use responsibly.

## Credits
Developed and maintained by [sathanicc](https://github.com/sathanicc).

## License
This project is licensed under the MIT License.
