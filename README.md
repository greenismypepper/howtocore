# howtocore 101

Installation:

  -Theres nothing strange in the installation of the core server, just the same as every Windows operative system
  -After finishing the installation, run the command "sconfig" and you will go to a option menu to configure the first steps before the server starts running.
  
  From here every configuration will be guided by the own sconfig.
  
Installing drivers in core server:
  1. Know your device: go to the builder's webpage to download the driver that you want to install in the server, in this case a multifunction Brother printer
  
  2. Decompress the drivers: use 7zip or other program to decompress the .exe in a folder, Something like "C:\Users\[Username]\Documents\[Name of the driver folder].
  
  3. Using PnPutil: use pnputil to install and add the drivers into the driverstore folder in system32, you must work with the .inf extension
  
        
          pnputil.exe -i -a  C:\Users\[username]\Documents\[Name of the driver folder]\[name].inf
          
  4. Adding folders to the driverstore var: 
