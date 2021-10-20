# HTB: Dancing
 
┌──(xnc㉿xnc-v8tpure)-[~]
└─$ smbclient -L 10.129.115.37
Enter WORKGROUP\xnc's password:

        Sharename       Type      Comment
        ---------       ----      -------
        ADMIN$          Disk      Remote Admin
        C$              Disk      Default share
        IPC$            IPC       Remote IPC
        WorkShares      Disk
SMB1 disabled -- no workgroup available


┌──(xnc㉿xnc-v8tpure)-[~]
└─$ smbclient  \\\\10.129.115.37\\ADMIN$
Enter WORKGROUP\xnc's password:
tree connect failed: NT_STATUS_ACCESS_DENIED

┌──(xnc㉿xnc-v8tpure)-[~]
└─$ smbclient  \\\\10.129.115.37\\C$
Enter WORKGROUP\xnc's password:
tree connect failed: NT_STATUS_ACCESS_DENIED

┌──(xnc㉿xnc-v8tpure)-[~]
└─$ smbclient  \\\\10.129.115.37\\Workshares$
Enter WORKGROUP\xnc's password:
tree connect failed: NT_STATUS_BAD_NETWORK_NAME

┌──(xnc㉿xnc-v8tpure)-[~]
└─$ smbclient  \\\\10.129.115.37\\WorkShares$
Enter WORKGROUP\xnc's password:
tree connect failed: NT_STATUS_BAD_NETWORK_NAME

┌──(xnc㉿xnc-v8tpure)-[~]
└─$ smbclient  \\\\10.129.115.37\\WorkShares
Enter WORKGROUP\xnc's password:
Try "help" to get a list of possible commands.


  #SMB  #Misconfiguration

