- SSH- Secure shell protocol is used btw devices in encrypted form. Using Cryptography , data is sent in encrypted form and then unencrypted once it reaches destinated device. 
- Two things needed for SSH : 1) IP address of remote machine 2) correct login credentials. 
- we can't see text when typing password in ssh login . 
- Majority of commands allow for the arguments to be provided. These arguments are identified by hyphens and certain words known as flags and switches. For example : ls shows folders in directory not hidden one. -a ( short form of all) . ls -a will show hidden folders as well. 
- files with "." are hidden files.
- --help will list of all possible commands.
- man command - manual pages. eg man ls - gives documentation of ls. .

- **Linux COMMANDS** :  1) Touch - create file 2 )mkdir - make directory - create a folder 3) cp-copy-Copy a file or folder 4) mv-move-Move a file or folder 5)  rm-remove- Remove a file or folder 6) file	-file	-Determine the type of a  file. 
- To remove file or directory we will using command rm . The command -> rm -R filename . -R is switch. 
- su command- used to switch btw users on linux . Things to know 1) user we wish to switch 2) user password . It will previous user home directory. 
- -l or --login . When used after su command , it will show current user home directory. eg su -l username. 
- /etc: root directory -etc folder  - used by operating system. 
- /var: variable data - folder stores data frequently used by services or applications. 
- /root - root user home directory.
- /tmp -stores temporary data . Once  computer restarted, temp data will be cleared  out. It is  useful in pentesting , good place to store enumeration scripts. 
- nano command - create new file and write multiple lines text in it. CTRL+X to exit . It will ask save , type Y and click enter to exit. 
- VIM is similar to nano but has more advanced features and works on all terminals. Type I for insert mode and press esc to exit insert mode. https://vim.rtorr.com/ for VIM cheatsheet. In VIM, command or normal mode allows you to use the commands. 
- wget command allows us to download images /files via web. Eg: wget https://assets.tryhackme.com/additional/linux-fundamentals/part3/myfile.txt.
- **scp** command is used to securely copy files between devices using ssh protocol. eg: scp important.txt ubuntu@192.168.1.30:/home/ubuntu/transferred.txt. 
- ubuntu comes with python3.
- process are the  programs running in the machine. PID is the id of the program. The PID increments for the order In which the process starts. I.e. the 60th process will have a PID of 60. **PS** command to see the processes running. To see the processes run by other users and those that don't run from a session use **ps aux** command.  
- **top** gives you real-time statistics about the processes running on your system instead of a one-time view. 
- To kill a command we use **kill** . Eg : kill PID number. To exit top command , just press **q**. 
- **systemctl** -- this command allows us to interact with the systemd. syntx : **systemctl [option] [service]**. EG : systemctl start apache2. 
- CRON: schedule a certain action or task to take place. Crontab is one of the processes that is started during boot, which is responsible for facilitating and managing cron jobs. https://crontab.guru/ AND https://crontab-generator.org/  - Resources to generate cron  commands. 
- **apt** command is used to install software. When adding software, the integrity of what we download is guaranteed by the use of what is called GPG (Gnu Privacy Guard) keys.
- **pwd**(print working directory) - means "show me the folder I'm currently in".
- ls- list of folders in current directory.
- ls -l details of folders in current directory.
- ls -al  it will display all the hidden files present in the directory. Hidden files start with .(dot).
- cd change directory or files. eg : cd Documents
- cat  : to read the content of the files . eg : cat filename
- uname : operating system name
- uname -a : To see details about the operating system, kernel version, and architecture.
- df -h : to check disk usage or available space.
- Linux stores configuration and informational files in the /etc directory.
- ssh username@ipaddress: To login as user and connect to computer using secure shell(ssh) .  eg : ss aashritha@1.1.1.1. This is used to connect computer remotely, run linux 
- su username(other) - to login as anotherusername in the same computer.
- **gobuster** - This fast directory/file and DNS brute-forcing tool helps in web security testing. It runs in terminal and automates in scanning web pages. syn gobuster dir -u http://example.com -w /path/to/wordlist.txt.  eg :
- “The grep command is used to search for specific words, text, or patterns inside files or command output.” eg: grep error logfile.txt.
- cd .. : go one level back.
- cd~ : go to home director
- find -name filename.txt : It will find the location of the text file. If we don't know the name of the file then use command find -name *.txt, it will provide all text files with path.
- wc filename : It counts lines , words and characters in the file. If we want lines only then w -l filename is the command. w -w filename : word count . w -m filename : character counter . w -c filename : bytes count.
- cat filename | wc -w  : Combined commands . First it gives output for first command and input of  the second command. | is called the pipe.
- grep -R "text" . : searches for text in all files /folders in current directory /folder. 
- touch filename.txt - To create new text file.
- nano filename.txt - To create and edit text file. If the file is already existed , it will let you to edit the file.
- lo      → internal system only
- enp0s3  → internet connection (important)
- inet    → your IP address
- man commandname - It gives manual page of that particular command. eg : man ls
- In Linux networking, UP means the network interface is enabled and active. It meant that the network card inside Ubuntu is turned on and ready to send/receive network traffic.
- sudo ss -tulpn : to get the ports that ubuntu listens on.
- stat filename : gives more detailed permissions of the file.
- ctrl+x to exit from nano editing screen.
- chown file  -  Only root. A normal user wants to change ownership of file from normal to root.
- sudo chown file  - normal user (but temporary acting as root) wants to change ownership to another user.
- su user - switch user .

- ** common directories **:
  1. /etc :  commonplace location to store system files that are used by your operating system. Contains user accounts, network settings and ssh coonfiguration. 
  2. /var : This folder stores data that is frequently accessed or written by services or applications running on the system. It contains logs and runtime data . Eg : /var/log, /var/www , /var/tmp. 
  3. /root : home directory of the root user.
  4. /tmp : Store data that is only needed to be accessed once or twice. Similar to the memory on your computer, once the computer is restarted, the contents of this folder are cleared out.
  5. /bin : Contains basic commands needed for all users. eg: ls, cp, mv, cat
  6. /sbin : System administration commands . Used by root /admin  only . eg : reboot , ipconfig, fdisk.
  7. /home : Each user gets personal home directory. eg /home/user1 , /home/user2
  8. /usr : User programs . It contains installed software. eg : /usr/bin ( user commands ) , /usr/data ( shared data ) , /usr/lib ( libraries).
  9. /opt : optional software : Used for installing third party apps.
  10. /dev : represents hardware . eg : /dev/sda - hard disk , /dev/usb : usb devices.
  11. /proc : processes information (virtual) : Not real files, generated in memory.
  12. /sys : Hardware and kernel information. Used to interact with hardware and kernel.
  13. /boot : Boot files. Contains system startup files. kernel and bootloader.
  14.  
- sudo ufw status - To check the firewall status. 




