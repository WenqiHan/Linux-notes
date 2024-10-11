# Linux notes
<<<<<<< Updated upstream
=======
Cybersecurity Notes

- `man [command]` to read the manual for any command.

Navigation in Linux
Commands List:
- ls
- cd
- pwd
- mkdir
- rmdir

- `ls`
  - Purpose: Lists the contents of a directory.
  - Usage: `ls` for basic listing, `ls -l` for detailed listing, `ls -a` to include hidden files.
  - Notes: Essential for quickly viewing what's in the current directory.

- `cd`
  - Purpose: Changes the current directory.
  - Usage: `cd [directory path]` to move to a specific directory, `cd ..` to move up one directory level, `cd` or `cd ~` to return to the home directory. `cd Documents` (relative path) cd /path/to/directory (absolute path)
  - Notes: Most commonly used for navigating through the filesystem.

- `pwd`
  - Purpose: Prints the current directory path.
  - Usage: `pwd` to display the full path of the current directory.
  - Notes: Useful for confirming your current location in the filesystem.

create:
- `mkdir`
  - Purpose: Creates a new directory.
  - Usage: `mkdir [directory name]` to create a new directory in the current location.
  - Notes: Handy for organizing files into new folders.

- `touch`
  - Purpose: make an empty file.
  - Usage: `touch newfile.txt` to make `newfile.txt`

Delete:
- `rmdir`
  - Purpose: Removes a directory.
  - Usage: `rmdir [directory name]` to delete an empty directory.
  - Notes: Used for cleaning up and removing unused directories. Note that the directory must be empty.

- `rm`
  - Purpose: remove a file
  - Usage: `rm -r` to remove a directory. `rm -r myfolder`Removes a directory and its contents recursively.

copy:
- `cp`
  - Purpose: copy files and directory
  - Usage: `cp file.txt /newfolder/` copies file to /newfolder/.

Move:
- `mv`
  - Purpose: move or rename file
  - usage: `mv oldname.txt newname.txt` renames the file.

Read:
- `cat`
  - Purpose: show what is in the file
  - Usage: `cat file.txt` shows file contents on the terminal.

- `less`
  - Purpose: allows you to scroll through a file.
  - Usage: `less filename.txt`
  - Notes: control -Z to exit.

Update:
- `nano`
  - Purpose: Opens a file in the Nano text editor.
  - Usage:`nano filename.txt` 
  - Notes: echo `"Text" &gt;&gt; filename.txt` Appends text to a file.
  

File permission:
 1. Use `ls -l` to view file permissions.
 2. Permissions are shown as -rwxrwxrwx
 Divided into User (u), Group (g), and Others (o).
 r — Read (4)
 w — Write (2)
 x — Execute (1)

chomd:
 Changing Permissions:
  - chmod u+x filename — Adds perform permission for the user.
  - chmod g-w filename — Removes write permission from the group.
  - chmod 755 filename — Sets permissions to rwxr-xr-x

Sudo:
  - `sudo [command]` Runs a command with superuser privileges. 
  - `sudo apt update` Updates package lists.
  - `sudo apt-get upgrade` Upgrade installed packages to the latest version.
  - `sudo apt-get install` Install new software packages.
  - `sudo apt-get install nmap` installs nmap tool.
  - `sudo apt-get remove` Remove software packages.
  - `sudo su` to get in 
  - `sudo nano /root/filename.txt` to create files
  - `sudo visudo` to check the sudoers
  - `sudo ls /root` to list files

- `su -` 
  - Notes: means swich user to root user which allows you to do more stuff

Networking:
- `ifconfig`
  - used either to assign network-interface or display current interface info

- `ip'
  - shows and manipulates routing, devies and tunnels

- `netstat`
  - uesd for configurations, troubleshooting, and monitoring over a network

- `iwconfig`
  - display and changes network parameters of the network interface, specific to the wireless operation
  - iwconfig `interface` [options]

- `traceroute`
  - traces ip address
  - traceroute `options`[hostname/ip]

- `tracepath`
  - shows the hop number, IP address or resolved hostname, and the round-trip time (RTT) for each hop
  - tracepath [options] [hostname/IP]

- `ping`
  - TCP command that checks connectivity, reachability, and name resolution
  - ping `options` host [hostname/ip]

- `mtr`
  - `my trace rout` sends real-time network quality checks
  - mtr [options] [hostname/IP]

- `tcpdump`
  - package sniffer/network security tool. analyzes network traffic, troubleshoots and monitors network
  - tcpdump [options] [filter]

- `ss`
  -shows all TCP sockets in the LISTEN state waiting for incoming connections.
  - ss [options] [filter]

- `whois`
  - queries network info and fetches domain ownership details
  - Ex: whois google.com

- `iftop`
  - views network connections and bandwidth usage in real time
  - primary usage: sudo iftop

- dig: interogates and looks up DNS servers
  - dig 'options' [domain] [record type] [DNS server]

- nslookup: offers fundamental DNS data
  - DNS lookup for domain: nslookup 'domain' 'DNS server'

- route: views and manipulates the IP routing table
  - route 'options' [subcommand] [arguments]

- host: looks up info through the DNS
  - host 'options' [hostname/IP]

- hostname: Displays and changes the system's hostname and domain. Identifies devices in a network
  - hostname 'options' [name] to control what the command displays
  - sudo hostname [name]: to temporarily change system hostname
            Check by running 'hostname' once more

- arp: displays IP-MAC address mapping
  - arp 'options' [hostname/IP]

Downloading files:
Commands that test downloading speeds
- wget: wget [options] [URL]
- curl: curl [options] [URL]

- `New-Item -ItemType File -Name "filename"`: to create a file in pwsh (ubuntu)
- `New-Item -ItemType Directory -Name "foldername"`: to create a folder (ubuntu)

>>>>>>> Stashed changes

