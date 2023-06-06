# Installing Virtualmin on Ubuntu 20.04 LTS Server

This guide provides step-by-step instructions on how to install Virtualmin, an open-source web hosting and cloud control panel, on an Ubuntu 20.04 LTS server. Virtualmin allows you to create and manage multiple hosting environments without the need to switch servers. It provides a secure and user-friendly interface, enabling server access through SSL-encrypted HTTP even with limited technical knowledge.

[![YouTube Video](https://img.youtube.com/vi/G2ZvhXH1SLs/maxresdefault.jpg)](https://youtu.be/G2ZvhXH1SLs)

## Prerequisites

Before proceeding with the installation, make sure you have completed the following prerequisites:

1. Deploy a fully updated Ubuntu 20.04 LTS server at Vultr.
2. Create a non-root user with sudo access.

## Installation Steps

Follow these steps to install Virtualmin on your Ubuntu 20.04 LTS server:

1. Download the Virtualmin installation script:

```
$ wget http://software.virtualmin.com/gpl/scripts/install.sh

```
2. Set the server's fully qualified domain name. Replace example.com with your desired domain:
```
$ sudo hostnamectl set-hostname example.com
```
3. Make the script executable:
```
$ chmod a+x install.sh
```
4. Run the installation script to install both Webmin and Virtualmin:
```
$ sudo ./install.sh
```
Note: The install.sh script provides various options for installation. You can refer to the script's help message for more details on available options.
5. Allow access to Virtualmin through the firewall:
```
$ sudo ufw allow 10000
```
6. Access the Virtual Web Interface by navigating to port 10000 on your server's fully qualified domain name. For example:
```
http://example.com:10000
```
## Conclusion
[![How to install Virtualmin / free hosting panel](https://github.com/khaleel-git/install-virtualmin-on-ubuntu-20-04/blob/master/Virtualmin%20github.png)](https://youtu.be/G2ZvhXH1SLs)
Congratulations! You have successfully installed Virtualmin on your Ubuntu 20.04 LTS server. To log in, use your server's root username and the password you set during the installation process. You can now access the Virtualmin Dashboard and begin configuring it to host websites. Enjoy the power and convenience of Virtualmin for your web hosting needs!
