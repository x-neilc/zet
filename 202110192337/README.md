# HTB: Fawn

nmap -sV 
    - Probe open ports to determine service/version info

Linux command-line ftp defaults to using active-mode FTP. Try switching to passive mode with the pass command:

me@ip-10-a-b-c:~$ ftp ftp.drupal.org
Name (ftp.drupal.org:me): anonymous
331 Please specify the password.
Password:
230 Login successful.
Remote system type is UNIX.
Using binary mode to transfer files.
ftp> dir
500 Illegal PORT command.
ftp: bind: Address already in use
ftp> pass
Passive mode on.
ftp> dir
227 Entering Passive Mode (140,211,166,134,86,192).
150 Here comes the directory listing.

  #FTP #'500 Illegal PORT Command'


