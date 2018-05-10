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

    Files:
        Create file     - touch 
        Remove file     - rm
        Rename a file   - mv
        Copy a file     - cp

    Directories:
        Linux Directory Structure
        / -> Root Directory 
        
        (Explore linux default directories and their purpose https://www.thegeekstuff.com/2010/09/linux-file-system-structure/ )
        Switch from one directory 
          $ cd
                1) `cd `-> Takes you to your home directory 
                2) `cd / ` -> Take you to `/` directory
                3) `cd -` -> Takes you to previous working directory
          $ pwd 

        Create Directory 
        Remove a Directory 
        Rename Directory 
        Copy a Directory 

        Move files from one dir to another
        Copy file from one dir to another
    Search Files & Directories:
    Utilities:
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


