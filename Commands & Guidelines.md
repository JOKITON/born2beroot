I have created a simple text file to sum up some of the most used commands & guidelines in born2beroot project.
All of this has been written and uploaded by @JOKITON, you can fork the repository and make any change you want.

Commands & Guidelines to use when evaluated:

HOSTNAME CHANGE:  sudo vi /etc/hostname -> sudo vi /etc/hosts -> sudo reboot

GROUPS: Some groups need to be created: sudo, user42. At least the user with login needs to be in both.
        sudo addgroup <group> -> sudo groupadd <user> <group> -> SUDO getent group <group>      
        sudo groupdel <group> -> sudo deluser <user> <group>  -> SUDO getent group <group>/<user>

USERS: An user with the login name has to exist.
        sudo adduser <user> -> SUDO getent user <user>
        sudo deluser <user> -> SUDO getent user <user>
       
SSH: Secure Shell, program used to access remote systems with safety.
        service ssh status / reload / stop / start / force-reaload / restart
        ssh -p <port> <username>@<ipadress>

UFW: Uncomplicated FIREWALL, a program that checks the activity going on and can take action if necessary.
        service ufw status / reload / stop / start / force-reaload / restart
        sudo ufw enable / disable / allow/deny <port> / status / reset / delete <number>

MONITORING.SH: Shell Script executed by crontab every 10 minutes.
        Working Directory : /root/monitoring.sh
        

SUDOERS: Group of certain users capable of executing commands with "sudo".
        su <user>
        Working Directory : etc/sudoers.d/sudoconfig
        Log Working Directory: var/log/sudo/sudo_log

CRON: SUDO crontab -e -> located in /var/spool/crontabs
        field          allowed values
              -----          --------------
              minute         0-59
              hour           0-23
              day of month   1-31
              month          1-12 (or names, see below)
              day of week    0-7 (0 or 7 is Sunday, or use names)

        
|                                                          BONUS                                                   |        
|------------------------------------------------------------------------------------------------------------------| 

|      NAME      |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------| 
|   `MARIADB`    |  DataBase Manager where we will create a database linked with an specific user.                 |

|    COMMANDS    |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------|        
| `sudo mariadb` | We open the command line of MariaDB from our terminal                                           |
|`show databases`| Shows all databases that are created                                                            |
| `drop database`| Deletes the database that is specified after the command                                        |
| `grant all on` | We create a new user with root privileges and with a password with this command                 |
| `sudo mysql_secure_installation` | Command that needs to be executed to set up MariaDB                           |
| `mysql -u` | Used to enter MariaDB terminal with the user we created before                                      |        

|----------------------------------------------------------------------------------------------------------------------------------------------------|
|----------------------------------------------------------------------------------------------------------------------------------------------------|
|----------------------------------------------------------------------------------------------------------------------------------------------------| 
        
|      NAME      |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------| 
|   `PHP`        |  Hypertext Preprocessor, open source code language useful for web programming.                  |

        
|----------------------------------------------------------------------------------------------------------------------------------------------------|
|----------------------------------------------------------------------------------------------------------------------------------------------------|
|----------------------------------------------------------------------------------------------------------------------------------------------------| 
       
|      NAME      |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------| 
|   `LIGHTTPD`    |  Web server aiming to be light, secure ... Easy configuration and good documentation.          |  
        
|    COMMANDS    |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------|        
|  `Port Number` | It needs to use the port number 80!                                                             |
|   `webroot`    | Uses the directory "/var/www/html"                                                              |
| `Modules conf` | "etc/lighttpd/conf-available/" / "etc/lighttpd/conf-enabled/"                                   |

|----------------------------------------------------------------------------------------------------------------------------------------------------|
|----------------------------------------------------------------------------------------------------------------------------------------------------|
|----------------------------------------------------------------------------------------------------------------------------------------------------|      
        
|      NAME      |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------| 
|  `WORDPRESS`   |  Free and open source blogging tool and a content management system based on PHP and MySQL.     |  
        
|    COMMANDS    |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------|        
|  `Working Directory` | "/etc/wordpress/config-"                                                                  |        
