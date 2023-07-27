### terminal nav 🐧
`CTRL + C` = exit current command
`COMMAND + K` = clear screen on mac
up and down arrows = generate previous commands
`open .` = open current folder you're in in finder

### file management 🗂️
`cd [path]` = go to path 
`ls` = list content of path
`mkdir ~/my_disk` = making a new directory
`touch example.txt` = create a new file of this name
`nano example.txt` = Edit a file using nano editor
`touch -t 200912150000.00 your_file_name` = Changing file date of a file
`mv index.html index2.html` = change file name from index.html to index2.html
`mv folder1 folder2` = this will move one folder1 to folder2
`open filename.html` = open file in default app
`open filename.html -a “Program Name”` = change the program used ... I don't use 
`rm -r directoryname` = remove all files in a directory
`rm directoryname` = just remove that one directory

### network 🌐
`ssh root@123.456.7.8 = Login to a server
`nslookup` = lookup IP for a domain. I used this often.
`whois domainname.com` = get who is info
`dig domain_name` = detailed information about DNS queries and responses
`host domainname.com` = I think this is similar to NSLookup
`sudo nano /etc/hosts` = file to map domains to IP
`cd /users/MyName/.ssh/` and then `rm known_hosts` = remove known hosts on mac
(many DNS related commands in this section)

### app install 📦
`sudo apt update ` = run this first
`sudo apt install proftpd` = sample install
`sudo apt remove proftpd` = remove install app (but it leaves config files)
`sudo apt purge proftpd` = totally remove it including the config files 

### app locations
Where files likely go when you install a typical app, using ProFTP as an example
`/etc/proftpd/` = config files. others: apache2, nginx, php, mysql, redis
`/usr/sbin/` = binary. others: same as above and also redis-server, memcached
`/usr/lib/proftpd/` = modules
`/var/log/proftpd/` = log files
`/home/username` = home directories
`/etc/init.d/` or `/lib/systemd/system/` = service script that allows you to start, stop, and restart the service

### disks/mount 💾
`sudo mount /dev/{disk_partition} /path/to/mount/point` = mounting it
`sudo umount /path/to/mount/point` = unmount it

### permissions
`ls -l filename` = view the permissions of a file
`chmod 644 filename` = change permissions for a file
`chmod -R <permissions> /path/to/folder` = change all permissions inside a folder

### memory 📝
`free` = output of how memory is currently allocated
`free -h` = more human readable format of the same

### disk
`df` = display table of disk usage on the system

### docker
`docker --version` = check version
`sudo service docker start` = start
`sudo service docker stop` = stop
`sudo service docker restart` = restart
`docker ps` = list all running containers
`docker ps -a` = List all containers (including stopped ones)
`docker start <container_name_or_id>` = To start a stopped container
`docker stop <container_name_or_id>` = To stop a running container
`docker restart <container_name_or_id>` = To restart a running container
`docker rm <container_name_or_id>` = To remove a stopped container
`docker rm -f <container_name_or_id>` = To stop and remove a running container in one command

### vhosts
`/etc/apache2/sites-available/example.com.conf` = common location for this

### php
`php [path/to/php/file]` = Execute a php file
`php -v` = check version
`sudo apache2ctl -M | grep php` = start
`/usr/lib/php/` = PHP extensions directory
`/etc/php/php.ini` = PHP configuration file

### mysql
`mysql --version` = check version
`sudo service mysql start` = start
`sudo service mysql stop` = stop
`sudo service mysql restart` = restart
`/var/lib/mysql/` = where MySQL data files are stored

### apache
`apache2 -v` = check version
`sudo service apache2 start` = start
`stop apache` = stop
`sudo service apache2 restart` = restart
`/var/www/html/` = web root directory

### ngnix
`nginx -v` = check version
`sudo service nginx start` = start
`sudo service nginx stop` = stop
`sudo service nginx restart` = restart
`/var/www/html/` = web root directory

### python
`python --version`
(Python is an interpreted language, so it doesn't have specific start/stop/reboot commands like server applications.)

### perl
`perl --version`
(Perl is a scripting language, so it doesn't have specific start/stop/reboot commands like server applications.)

### proftp
`proftpd -v` = check version (or `proftpd --version`)
`sudo service proftpd start` = start
`sudo service proftpd stop` = stop
`sudo service proftpd restart` = restart

### redis
`redis-server --version` = check version
`sudo service redis-server start` = start
`sudo service redis-server stop` = stop
`sudo service redis-server restart` = restart

### memcached
`memcached -h | grep "memcached -"` = check version
`sudo service memcached start` = start
`sudo service memcached stop` = stop
`sudo service memcached restart` = restart


## Ubuntu folders
### /bin
Essential executable binaries (commands) that are required for basic system functioning. These binaries are accessible to all users.

### /boot
Contains the kernel, initial RAM disk, and other boot-related files used during the boot process.

### /dev
Provides access to device files that represent hardware devices, such as disks, partitions, terminals, etc.

### /etc
Contains system-wide configuration files. Important settings for various software and services are stored here.
#### /etc/crontab
A shell script to run specified commands on a predefined time Interval.

### /home
The home directories for regular users are located here. Each user typically has a subdirectory within /home for their personal files and configurations.

### /lib and /lib64
These directories hold essential shared library files that are used by the system and various applications.

### /media
Traditionally used for mounting removable media such as USB drives, CDs, DVDs, etc.

### /mnt
Used for temporarily mounting filesystems or other devices.

### /opt
Often used for installing additional software packages or applications that are not part of the default system.

### /proc
A virtual filesystem that provides information about running processes and system status. It is not an actual disk directory but a way to interact with the kernel.

### /root
The home directory for the root user, the superuser with administrative privileges.

### /run
Used for storing temporary data related to the currently running system.

### /sbin
Contains system binaries, primarily used by the system administrator.

### /srv
Typically used to store data for services provided by the system.

### /sys
Similar to /proc, it provides information about the kernel and devices. It is also not an actual disk directory.

### /tmp
Used for storing temporary files that are typically cleared on system reboot.

### /usr
Contains user-related files, including executable binaries, libraries, documentation, and more.

### /var
Holds variable data, such as log files, spool files, and temporary files generated by various services.

## More info
[[Code-Linux-Ubuntu-Ref]]


