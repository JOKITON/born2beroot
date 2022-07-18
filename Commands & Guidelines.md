|I have created a simple text file to sum up some of the most used commands & guidelines in born2beroot project.|
|------------------------------------------------------------------------------------------------------------------|
|All of this has been written and uploaded by @JOKITON, you can fork the repository and make any change you want.|

|                   Commands & Guidelines to use when evaluated:                                                   |        
|------------------------------------------------------------------------------------------------------------------|

|      NAME      |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------| 
|   `HOSTNAME`   |The hostname is a label that is assigned to a device connected to a computer network.            |

|  INFORMATION   |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------|        
| `Hostname Path`| /etc/hostname                                                                                   |
|  `Hosts Path`  | /etc/hosts                                                                                      |

|----------------------------------------------------------------------------------------------------------------------------------------------------|
|----------------------------------------------------------------------------------------------------------------------------------------------------|

|      NAME      |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------| 
|   `GROUPS`     | Some groups need to be created: sudo, user42. At least the user with login needs to be in both. |

|    COMMANDS    |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------|        
| `sudo addgroup`| Used to create a new group in the system.                                                       |
|`sudo groupadd` | Used to add a user to a group / create a new group in the system.                               |
| `sudo groupdel`| Used to delete a group from the system.                                                         |
| `sudo deluser` | Used to delete a user from a group / delete an user from the system.                            |   
| `getent group` | Lists all groups and users of the system.                                                       |

|----------------------------------------------------------------------------------------------------------------------------------------------------|
|----------------------------------------------------------------------------------------------------------------------------------------------------|

|      NAME      |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------| 
|    `USERS`     | A user often has a user account and is identified to the system by a username.                  |

|    COMMANDS    |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------|        
| `sudo adduserr`| Used to create a new user in the system.                                                        |
| `sudo deluser` | Used to delete a user from a group / delete an user from the system.                            |   
| `getent group` | Lists all groups and users of the system.                                                       |

|----------------------------------------------------------------------------------------------------------------------------------------------------|
|----------------------------------------------------------------------------------------------------------------------------------------------------|
       
|      NAME      |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------| 
|     `SSH`      | Secure Shell, program used to access remote systems with safety.                                |

|    COMMANDS    |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------|   
|  `service ssh` | It can be used to see the status, stop the service, restart it...                               |
|`service <...>` | status / reload / stop / start / force-reaload / restart                                        |
|    `ssh -p`    | Used to connect to a remote system through SSH.                                                 |   

|----------------------------------------------------------------------------------------------------------------------------------------------------|
|----------------------------------------------------------------------------------------------------------------------------------------------------|


|      NAME      |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------| 
|     `UFW`      | Uncomplicated FIREWALL, a program that checks the activity going on and can take action if necessary.            |

|    COMMANDS    |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------|   
|  `service ufw` | It can be used to see the status, stop the service, restart it...                               |
|`service <...>` | status / reload / stop / start / force-reaload / restart                                        |
|   `sudo ufw`   | You can see the ports that are open , allow/deny ports, reset...                                | 
|`sudo ufw <...>`| enable / disable / allow/deny <port> / status / reset / delete <number>                         |   

|----------------------------------------------------------------------------------------------------------------------------------------------------|
|----------------------------------------------------------------------------------------------------------------------------------------------------|

|      NAME      |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------| 
|`MONITORING.SH` | Shell Script that shoudl be executed by crontab every 10 minutes.                               |

|    COMMANDS    |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------|   
|`Working Directory`| /root/monitoring.sh                                                                          |

|----------------------------------------------------------------------------------------------------------------------------------------------------|
|----------------------------------------------------------------------------------------------------------------------------------------------------|
        
|      NAME      |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------| 
|   `SUDOERS`    | Group of certain users capable of executing commands with "sudo".                               |

|    COMMANDS    |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------|   
|   `su <user>`  | Used to switch the user we are currently using.                                                 |
|`Working Directory` | etc/sudoers.d/sudoconfig                                        |
|   `Log Working Directory`   | var/log/sudo/sudo_log                                | 

|----------------------------------------------------------------------------------------------------------------------------------------------------|
|----------------------------------------------------------------------------------------------------------------------------------------------------|     
        
|      NAME      |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------| 
|     `CRON`      | The cron command-line utility is a job scheduler on Unix-like operating systems.               |

|    COMMANDS    |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------|   
|  `crontab -e`  | Used to edit the crontab file.                                                                  |
|`Cron Directory`| /var/spool/crontabs                                                                   |    
        
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
        
|      NAME      |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------| 
|   `PHP`        |  Hypertext Preprocessor, open source code language useful for web programming.                  |

        
|----------------------------------------------------------------------------------------------------------------------------------------------------|
|----------------------------------------------------------------------------------------------------------------------------------------------------|
       
|      NAME      |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------| 
|   `LIGHTTPD`    |  Web server aiming to be light, secure ... Easy configuration and good documentation.          |  
        
|   INFORMATION  |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------|        
|  `Port Number` | It needs to use the port number 80!                                                             |
|   `webroot`    | Uses the directory "/var/www/html"                                                              |
| `Modules conf` | "etc/lighttpd/conf-available/" / "etc/lighttpd/conf-enabled/"                                   |

|----------------------------------------------------------------------------------------------------------------------------------------------------|
|----------------------------------------------------------------------------------------------------------------------------------------------------|   
        
|      NAME      |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------| 
|  `WORDPRESS`   |  Free and open source blogging tool and a content management system based on PHP and MySQL.     |  
        
|  INFORMATION   |                                      DESCRIPTION                                                |
|----------------|-------------------------------------------------------------------------------------------------|        
|  `Working Directory` | "/etc/wordpress/config-"                                                                  |        
