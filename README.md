# S.E.A.
S.E.A. - Space Engineer Assistant, Workshop mod for the game "Space Engineers" 

My working version from https://github.com/OniVe/S.E.A./releases  
Original mod link in Steam Workshop (doesn't work) https://steamcommunity.com/sharedfiles/filedetails/?id=680600621

![Work example 1](https://github.com/Twertoon/SEA/blob/master/gif%20example/ezgif.com-gif-maker.gif)  
![Work example 2](https://github.com/Twertoon/SEA/blob/master/gif%20example/ezgif.com-gif-maker%20(1).gif)

###   Server installation *(Steam client)*:
1.  Download the server **SEA.P** (and game MOD **SEA.GM**)
2.  Unpack the archive file
3.  Go to the Steam client
4.  Menu **"Library"** -> press the right mouse button on the game **"Space Engineers"** -> Properties
5.  In the window **"Space Engineers - Properties"** select the **"Local files"** tab
6.  On the Advanced tab click **"BROWSE LOCAL FILES"**
7.  In the Explorer window, go to the folder **"Bin64"** and copy into it the contents of the directory **"SEA.P"** from the unpacked archive
8.  Close the Explorer window
9.  In the window **"Space Engineers - Properties"** select the **"General"** tab
10. Press the **"SET LAUNCH OPTIONS..."**
11. In the window **"Parameters of run - Space Engineers"** in the input box to insert a line **" -plugin SEA.P.dll"**
12. Press button **"OK"**

###   Server configuration:
1.  Set the port (if necessary) [9000 by default]
 *  Open file **"SEA.P.dll.config"** located in the directory of the game **".\Bin64"** via notepad
 *  Change the value to the desired value 9000 on the **<add key = "port" value = "9000" />**
2.  Add inbound and outbound rule to selected port in firewall

###   The order of updating from the old version:
1.  Delete the directory **"web"** in the root directory of the server **"SEA.P.dll"**  (.\Bin64)
2.  Copy the configuration file **"storage.s3db"** in the directory **".\Bin64"**

##   ! Warning !
* If you run the MOD (**SEA.GM**) without connected plugin server (**SEA.P.dll**), it is raise an **error** when you try to save the game. ***(Saving files will not be damaged)***.