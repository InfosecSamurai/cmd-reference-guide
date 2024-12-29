![rsz_2enwni1b](https://github.com/user-attachments/assets/8253940e-2549-4be1-836c-6eb81fe771d2)



# Command Prompt (CMD) Reference Guide

This guide provides a comprehensive list of Windows Command Prompt (cmd) commands, including basic commands, additional commands, and commands commonly used by ethical hackers and penetration testers.

[CMD Reference Guide](https://infosecsamurai.github.io/cmd-reference-guide)

## Table of Contents

1. [Basic Commands](#basic-commands)
2. [Additional Commands](#additional-commands)
3. [Commands for Ethical Hackers and Pentesters](#commands-for-ethical-hackers-and-pentesters)
4. [Secret Commands](#secret-commands)
5. [Usage Tips](#usage-tips)

## Basic Commands

### CD
- **Description**: Changes the current directory to the specified path.
- **Usage**:
   ```cmd
   CD C:\\Users\\Username\\Documents

- **Example Output**:
(No output, but the prompt changes to indicate the new directory.)

### DIR

- **Description**: Lists the contents of a directory.
- **Usage**:
    
    ```cmd
    DIR
    ```
    
- **Example Output**:
    
    ```
    Volume in drive C has no label.
    Volume Serial Number is XXXX-XXXX
    
    Directory of C:\\Users\\Username\\Documents
    
    12/17/2024  10:00 AM    <DIR>          .
    12/17/2024  10:00 AM    <DIR>          ..
    12/17/2024  09:00 AM                 123 example.txt
    ```
    

### COPY

- **Description**: Copies files from one location to another.
- **Usage**:
    
    ```
    COPY C:\\source\\file.txt D:\\destination\\
    ```
    
- **Example Output**:
    
    ```
    1 file(s) copied.
    ```
    

### DEL

- **Description**: Deletes one or more files.
- **Usage**:
    
    ```
    DEL C:\\Users\\Username\\Documents\\file.txt
    ```
    
- **Example Output**:
    
    ```
    1 file(s) deleted.
    ```
    

### REN

- **Description**: Renames a file or directory.
- **Usage**:
    
    ```
    REN oldfilename.txt newfilename.txt
    ```
    
- **Example Output**:
(No output, but the file is renamed.)

### MD

- **Description**: Creates a new directory.
- **Usage**:
    
    ```
    MD NewFolder
    ```
    
- **Example Output**:
(No output, but the folder is created.)

### RD

- **Description**: Removes a directory.
- **Usage**:
    
    ```
    RD NewFolder
    ```
    
- **Example Output**:
(No output, but the folder is removed.)

### CLS

- **Description**: Clears the Command Prompt screen.
- **Usage**:
    
    ```
    CLS
    ```
    
- **Example Output**:
(No output, the screen is cleared.)

### EXIT

- **Description**: Exits the Command Prompt.
- **Usage**:
    
    ```
    EXIT
    ```
    
- **Example Output**:
(No output, the Command Prompt window closes.)

### ECHO

- **Description**: Displays messages or turns command echoing on or off.
- **Usage**:
    
    ```
    ECHO Hello, World!
    ```
    
- **Example Output**:
    
    ```
    Hello, World!
    ```
    

## Additional Commands

### ASSOC

- **Description**: Displays or modifies file extension associations.
- **Usage**:
    
    ```
    ASSOC .txt
    ```
    
- **Example Output**:
    
    ```
    .txt=txtfile
    ```
    

### CHCP

- **Description**: Changes the active code page number.
- **Usage**:
    
    ```
    CHCP
    ```
    
- **Example Output**:
    
    ```
    Active code page: 437
    ```
    

### CHOICE

- **Description**: Accepts user input from a set of choices.
- **Usage**:
    
    ```
    CHOICE /C ABC /N "Choose A, B, or C:"
    ```
    
- **Example Output**:
    
    ```
    Choose A, B, or C:
    ```
    

### COLOR

- **Description**: Sets the default console foreground and background colors.
- **Usage**:
    
    ```
    COLOR 0A
    ```
    
- **Example Output**:
  (No output, but the text color changes to green on a black background.)


### COMP

- **Description**: Compares the contents of two or more files.
- **Usage**:
    
    ```
    COMP file1.txt file2.txt
    ```
    
- **Example Output**:
    
    ```
    Files file1.txt and file2.txt are identical.
    ```
    

### DISKSHADOW

- **Description**: Manages shadow copies.
- **Usage**:
    
    ```
    DISKSHADOW
    ```
    
- **Example Output**:
(Enters the Diskshadow command prompt.)

### FIND

- **Description**: Searches for a text string in a file or files.
- **Usage**:
    
    ```
    FIND "search_string" file.txt
    ```
    
- **Example Output**:
    
    ```
    1: This is the line with the search_string.
    ```
    

### LABEL

- **Description**: Creates or changes the label of a disk.
- **Usage**:
    
    ```
    LABEL D: NewLabel
    ```
    
- **Example Output**:
(No output, but the label is changed.)

### NBTSTAT

- **Description**: Displays NetBIOS over TCP/IP statistics.
- **Usage**:
    
    ```
    NBTSTAT -s
    ```
    
- **Example Output**:
    
    ```
    Host Table
    Name            Type         Status
    ------------------------------------------
    MyComputer      <00>        Registered
    ```
    

### POWERCFG

- **Description**: Configures power settings.
- **Usage**:
    
    ```
    POWERCFG /LIST
    ```
    
- **Example Output**:
    
    ```
    Power Schemes (*) are Labeled.
    ```
    

### RECYCLER

- **Description**: Manages the Recycle Bin (deprecated).
- **Usage**:
    
    ```
    RECYCLER
    ```
    
- **Example Output**:
(No output; used in legacy systems.)

### SC

- **Description**: Communicates with the Service Control Manager.
- **Usage**:
    
    ```
    SC QUERY
    ```
    
- **Example Output**:
    
    ```
    SERVICE_NAME: wuauserv
    DISPLAY_NAME: Windows Update
    ```
    

### SETX

- **Description**: Sets environment variables permanently.
- **Usage**:
    
    ```
    SETX MY_VAR "My Value"
    ```
    
- **Example Output**:
    
    ```
    SUCCESS: Specified value was saved.
    ```
    

### TIMEOUT

- **Description**: Delays processing for a specified period.
- **Usage**:
    
    ```
    TIMEOUT 5
    ```
    
- **Example Output**:
    
    ```
    Waiting for 5 seconds, press a key to continue...
    ```
    

### NET TIME

- **Description**: Synchronizes the computer's clock with a network time source.
- **Usage**:
    
    ```
    NET TIME \\\\timeserver
    ```
    
- **Example Output**:
    
    ```
    The current time is 10:00 AM.
    ```
    

## Commands for Ethical Hackers and Pentesters

### IPCONFIG

- **Description**: Displays network configuration for all network adapters.
- **Usage**:
    
    ```
    IPCONFIG
    ```
    
- **Example Output**:
    
    ```
    Windows IP Configuration
    
    Ethernet adapter Ethernet:
        Connection-specific DNS Suffix  . : example.com
        IPv4 Address. . . . . . . . . . . . : 192.168.1.2
        Subnet Mask . . . . . . . . . . . . : 255.255.255.0
        Default Gateway . . . . . . . . . . . : 192.168.1.1
    ```
    

### PING

- **Description**: Checks connectivity to a network host.
- **Usage**:
    
    ```
    PING google.com
    ```
    
- **Example Output**:
    
    ```
    Pinging google.com [216.58.214.206] with 32 bytes of data:
    Reply from 216.58.214.206: bytes=32 time=14ms TTL=117
    ```
    

### TRACERT

- **Description**: Traces the path to a network host.
- **Usage**:
    
    ```
    TRACERT google.com
    ```
    
- **Example Output**:
    
    ```
    Tracing route to google.com [216.58.214.206]
    over a maximum of 30 hops:
       1    <1 ms    <1 ms    <1 ms  router.local [192.168.1.1]
       2     10 ms     9 ms     8 ms  10.10.10.1
    ```
    

### NETSTAT

- **Description**: Shows active connections and listening ports.
- **Usage**:
    
    ```
    NETSTAT -an
    ```
    
- **Example Output**:
    
    ```
    Proto  Local Address          Foreign Address        State
    TCP    0.0.0.0:135           0.0.0.0:0             LISTENING
    ```
    

### NSLOOKUP

- **Description**: Queries DNS records.
- **Usage**:
    
    ```
    NSLOOKUP google.com
    ```
    
- **Example Output**:
    
    ```
    Server:  dns.server.com
    Address:  192.168.1.1
    
    Non-authoritative answer:
    Name:    google.com
    Addresses:  216.58.214.206
    ```
    

### ARP

- **Description**: Displays the ARP table.
- **Usage**:
    
    ```
    ARP -a
    ```
    
- **Example Output**:
    
    ```
    Interface: 192.168.1.2 --- 0x2
        Internet Address      Physical Address      Type
        192.168.1.1          00-14-22-01-23-45     dynamic
    ```
    

### NET VIEW

- **Description**: Lists shared resources on a network.
- **Usage**:
    
    ```
    NET VIEW
    ```
    
- **Example Output**:
    
    ```
    Shared resources at \\\\COMPUTERNAME
    Share name   Type   Comment
    ----------------------------------------------------
    Documents    Disk   My Documents
    ```
    

### NET USER

- **Description**: Displays or modifies user account information.
- **Usage**:
    
    ```
    NET USER
    ```
    
- **Example Output**:
    
    ```
    User accounts for \\\\COMPUTERNAME
    -------------------------------------------------------------------------------
    Administrator            Guest
    User1                    User2
    The command completed successfully.
    ```
    

### WHOAMI

- **Description**: Displays the current user and its groups.
- **Usage**:
    
    ```
    WHOAMI
    ```
    
- **Example Output**:
    
    ```
    Username
    ```
    

### SYSTEMINFO

- **Description**: Retrieves detailed system information.
- **Usage**:
    
    ```
    SYSTEMINFO
    ```
    
- **Example Output**:
    
    ```
    Host Name:                 COMPUTERNAME
    OS Name:                   Microsoft Windows 10 Pro
    OS Version:                10.0.19041 N/A Build 19041
    ```
    

### WMIC

- **Description**: Accesses system information and management tasks.
- **Usage**:
    
    ```
    WMIC CPU GET Name
    ```
    
- **Example Output**:
    
    ```
    Name
    Intel(R) Core(TM) i7-8700 CPU @ 3.20GHz
    ```
    

### DIR

- **Description**: Lists directory contents.
- **Usage**:
    
    ```
    DIR
    ```
    
- **Example Output**:
    
    ```
    Volume in drive C has no label.
    Volume Serial Number is XXXX-XXXX
    
    Directory of C:\\Users\\Username\\Documents
    ```
    

### COPY

- **Description**: Copies files from one location to another.
- **Usage**:
    
    ```
    COPY C:\\source\\file.txt D:\\destination\\
    ```
    
- **Example Output**:
    
    ```
    1 file(s) copied.
    ```
    

### MOVE

- **Description**: Moves files from one location to another.
- **Usage**:
    
    ```
    MOVE C:\\source\\file.txt D:\\destination\\
    ```
    
- **Example Output**:
    
    ```
    1 file(s) moved.
    ```
    

### DEL

- **Description**: Deletes one or more files.
- **Usage**:
    
    ```
    DEL C:\\Users\\Username\\Documents\\file.txt
    ```
    
- **Example Output**:
    
    ```
    1 file(s) deleted.
    ```
    

### ICACLS

- **Description**: Modifies file and directory permissions.
- **Usage**:
    
    ```
    ICACLS file.txt /grant UserName:F
    ```
    
- **Example Output**:
    
    ```
    processed file: file.txt
    Successfully processed 1 files; Failed processing 0 files
    ```
    

### NET LOCALGROUP

- **Description**: Manages local user groups.
- **Usage**:
    
    ```
    NET LOCALGROUP Administrators
    ```
    
- **Example Output**:
    
    ```
    Alias name     Administrators
    Comment        Administrators have complete and unrestricted access to the computer/domain
    ```
    

### ROBOCOPY

- **Description**: Robust file copy, useful for transferring files.
- **Usage**:
    
    ```
    ROBOCOPY C:\\source D:\\destination /E
    ```
    
- **Example Output**:
    
    ```
    100% New File              1        10.00 k    file.txt
    ```
    

### SHUTDOWN

- **Description**: Shuts down or restarts the computer.
- **Usage**:
    
    ```
    SHUTDOWN /r /t 0
    ```
    
- **Example Output**:
(No output; the computer will restart immediately.)

### TASKLIST

- **Description**: Lists running processes.
- **Usage**:
    
    ```
    TASKLIST
    ```
    
- **Example Output**:
    
    ```
    Image Name                     PID Session Name        Session#    Mem Usage
    ========================= ======== ================ =========== ============
    cmd.exe                       1234 Console                    1     10,000 K
    ```
    

### TASKKILL

- **Description**: Terminates processes.
- **Usage**:
    
    ```
    TASKKILL /PID 1234 /F
    ```
    
- **Example Output**:
    
    ```
    SUCCESS: The process with PID 1234 has been terminated.
    ```
    

### NETSH

- **Description**: Configures network settings.
- **Usage**:
    
    ```
    NETSH WLAN show profiles
    ```
    
- **Example Output**:
    
    ```
    Profiles on interface Wi-Fi :
    Group policy profiles (read only) :
    ------------------------------------
    <None>
    
    User profiles :
    -------------------
    Profile 1
    ```
    

### CIPHER

- **Description**: Manages file encryption and decryption.
- **Usage**:
    
    ```
    CIPHER /E file.txt
    ```
    
- **Example Output**:
    
    ```
    Successfully encrypted:  file.txt
    ```
    

## Secret Commands

### HELP

- **Description**: Lists all available commands.
- **Usage**:
    
    ```
    HELP
    ```
    
- **Example Output**:
    
    ```
    ASSOC           Displays or modifies file extension associations
    CD              Displays the name of or changes the current directory
    ```
    

### NET USE

- **Description**: Connects or disconnects from a shared resource.
- **Usage**:
    
    ```
    NET USE Z: \\\\Server\\Share
    ```
    
- **Example Output**:
    
    ```
    The command completed successfully.
    ```
    

### NTRIGHTS

- **Description**: Manages user rights and privileges.
- **Usage**:
    
    ```
    NTRIGHTS +r SeDenyNetworkLogonRight -u UserName
    ```
    
- **Example Output**:
    
    ```
    Success
    ```
    

### VER

- **Description**: Displays the Windows version.
- **Usage**:
    
    ```
    VER
    ```
    
- **Example Output**:
    
    ```
    Microsoft Windows [Version 10.0.19041.928]
    ```
    

### WHOAMI

- **Description**: Displays the current username and group memberships.
- **Usage**:
    
    ```
    WHOAMI /ALL
    ```
    
- **Example Output**:
    
    ```
    USER: DOMAIN\\UserName
    GROUP: Everyone
    ```
    

### SYSTEMINFO

- **Description**: Provides detailed system information.
- **Usage**:
    
    ```
    SYSTEMINFO
    ```
    
- **Example Output**:
    
    ```
    Host Name:                 COMPUTERNAME
    OS Name:                   Microsoft Windows 10 Pro
    ```
    

### FSUTIL

- **Description**: Perform tasks related to file systems.
- **Usage**:
    
    ```
    FSUTIL FSINFO drives
    ```
    
- **Example Output**:
    
    ```
    Drives: C: D:
    ```
    

### OPENFILES

- **Description**: Displays files opened by remote users.
- **Usage**:
    
    ```
    OPENFILES
    ```
    
- **Example Output**:
    
    ```
    There are no open files on this system.
    ```
    

### WMIC

- **Description**: Accesses system information and management tasks.
- **Usage**:
    
    ```
    WMIC PROCESS LIST
    ```
    
- **Example Output**:
    
    ```
    Handle  ProcessId  Name
    1234    5678       notepad.exe
    ```
    

## Usage Tips

- Always run Command Prompt as an administrator for commands that require elevated privileges.
- Use the `/help` option with commands to learn more about their usage.
- Be cautious when using commands that modify system settings or files.
