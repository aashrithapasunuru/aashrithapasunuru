SSH- Secure shell protocol is used btw devices in encrypted form. Using Cryptography , data is sent in encrypted form and then unencrypted once it reaches destinated device. 
two things needed for SSH : 1) IP address of remote machine 2) correct login credentials. 
we can't see text when typing password in ssh login . 
Majority of commands allow for the arguments to be provided. These arguments are identified by hyphens and certain words known as flags and switches. For example : ls shows folders in directory not hidden one. -a ( short form of all) . ls -a will show hidden folders as well. 
files with "." are hidden files.
--help will list of all possible commands.
man command - manual pages. eg man ls - gives documentation of ls. 
COMMANDS :  1) Touch - create file 2 )mkdir - make directory - create a folder 3) cp-copy-Copy a file or folder 4) mv-move-Move a file or folder 5)  rm-remove- Remove a file or folder 6) file	-file	-Determine the type of a  file. 
To remove file or directory we will using command rm . The command -> rm -R filename . -R is switch. 
su command- used to switch btw users on linux . Things to know 1) user we wish to switch 2) user password . It will previous user home directory. 
-l or --login . When used after su command , it will show current user home directory. eg su -l username. 
/etc: root directory -etc folder  - used by operating system. 
/var: variable data - folder stores data frequently used by services or applications. 
/root - root user home directory.
/tmp -stores temporary data . Once  computer restarted, temp data will be cleared  out. It is  useful in pentesting , good place to store enumeration scripts. 
nano command - create new file and write multiple lines text in it. CTRL+X to exit . It will ask save , type Y and click enter to exit. 
VIM is similar to nano but has more advanced features and works on all terminals. Type I for insert mode and press esc to exit insert mode. https://vim.rtorr.com/ for VIM cheatsheet. 


