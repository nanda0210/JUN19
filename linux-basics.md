
```
Linux:

  Basic:
    System Info:
        H/W
            - CPU
                $ cat /proc/cpuinfo
            - MEM 
                $ cat /proc/meminfo
            - DISK 
                $ sudo fdisk -l
        S/W
            - OS Vendor
            - OS Version
                $ cat /etc/*release
            - OS Arch
                $ uname -i 
                x86_64/x64              -> 64 bit 
                x86/i386,i586,i686      -> 32 bit
   
    User Notations:
      $ -> Normal User
      # -> Root User
      
    Linux Command Syntax:
        command-name {options} {inputs}
            ex: uname
                uname -i 
                cat /proc/cpuinfo

            Options:
                -(single character) , -i -x, -s
                --(single word) , --help, --verbose

            Default option for all commands : --help

    Linux Commands help:

    List files & Dir: 
        $ ls
        $ ls -l     <-- Shows long list
        
        Type of file can be determined by ls -l command and the first character denotes that.
          - -> Regular File
          d -> directory 
        Note: There are total 7 types of files, Explore them.
        
    Files:
        Create file     - touch 
        Remove file     - rm
        Rename a file   - mv
          $ mv source target
            1) If target does not exist ??
              Rename the file 
            2) If target exists ??
              Overwrite the file (1. Remove target , 2. Rename Source to target )
            3) If target exists and if it is a directory.
              Moves file into target directory 
        Copy a file     - cp

    Directories:
        Linux Directory Structure
        / -> Root Directory 
        
        (Explore linux default directories and their purpose https://www.thegeekstuff.com/2010/09/linux-file-system-structure/ )
        Switch from one directory 
          $ cd
                1) cd  -> Takes you to your home directory 
                2) cd / -> Take you to `/` directory
                3) cd - -> Takes you to previous working directory
                4) cd ..  -> Takes to parent directory (.. denotes parent directory,   . denotes present directory)
                
          $ pwd 

        Create Directory 
          $ mkdir dir-name
        Remove a Directory 
          $ rm  -r dir-name
        Rename Directory 
          $ mv dir-name new-dir-name
              1) If new-dir-name does not exist ?? 
                  It is just renaming directory 
              2) If new-dir-name already exists ??
                  It is going to move the directory into new-dir-name
                  
        Copy a Directory 
          $ cp -r source-dir remote-dir
          
        Move files from one dir to another
        Copy file from one dir to another
    
    Editor:
      ->  vi / vim / nano / gedit 
      *** vi / vim 
```
Image of VI Editor:
![image](https://user-images.githubusercontent.com/29029753/39901770-3a6d9154-54e8-11e8-8d7a-a7ff52ce7d4f.png)



```   
    Search Files & Directories:
      1. Find Command.  
          $ find /etc "*.conf"
          $ find /home/ec2-user -name "*.conf" -type f
          $ find /home/ec2-user -name "*.conf" -type d
          
      2. Locate command.
         locate command will not be there by default , hence lets install and use it.
          $ sudo yum install mlocate -y
          $ sudo updatedb
          
          $ locate "*.conf"
          $ locate "*.conf" | grep /home
    Filter Commands:
      Perform this command before going with commands.
        $ sudo cp /var/log/messages .;sudo chmod 666 messages
      -> cat 
        $ cat messages
      -> wc 
        $ wc -l  messages
        $ wc -c  messages
      -> head
        $ head messages
        $ head -2 messages
      -> tail 
        $ tail messages
        $ tail -n 2 messages
      -> grep 
        $ grep yum messages 
        $ grep yum messages
      -> cut
        $ cut -d ':' -f 1 /etc/passwd
      
    Utilities:
      wget command is nott there by default in linux, Hence install it.
      $ sudo yum install wget -y
      -> wget 
        $ wget http://www-eu.apache.org/dist//httpd/httpd-2.4.33.tar.gz
        
      -> curl 
        Curl is command to browse over CLI.
        $ curl 
        
      -> tar 
      
      -> Pipes
      
  Admin:
    Package Management:
    Service Management:
    User Management:
        - Users
        - Groups
        - Sudoers
        - File/Dir Permissions
    
    Disk Management:
    Network Management:

```
