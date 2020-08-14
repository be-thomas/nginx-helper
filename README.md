# nginx-helper

## Dependencies
Make sure you have python3, wget installed \
On ubuntu, debian, kali you use this command to install \
> `sudo apt install python3 wget`
On CentOS use - \
> `yum install python3 wget` \
On Arch Linux use - \
> `pacman -S python3 wget` \

## Installation
Run below commands in order -
    `wget -O nginx-helper https://raw.githubusercontent.com/thomasb892/nginx-helper/master/nginx-helper
    chmod +x nginx-helper
    sudo mv nginx-helper /usr/bin/nginx-helper`

## Usage
After installation, you can start using 'nginx-helper'
Use the below command to create a new site(replace) -
    `nginx-helper new`
To view all sites type the command below -
    `nginx-helper sites`
To disable a site, type this command then choose from the list of enabled sites -
    `nginx-helper disable`
Use the command below command to enable a site -
    `nginx-helper enable`
For deleting a site, use -
    `nginx-helper delete`


if you want to create a site which only listen to ipv4 -
    `nginx-helper new [domain-name] -ipv4 y -ipv6 n`
Creating a site with only ipv6 -
    `nginx-helper new [domain-name] -ipv6 y -ipv4 n`
Creating a site which listens to a different port, Something other than port 80 -
    `nginx-helper new [domain-name] -port [port-number]`
