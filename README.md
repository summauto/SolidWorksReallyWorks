# How to install

1. Get the installation files, either from..
   1. a torrent `DS.SolidWorks.2020.SP0.Premium.torrent`, or
   2. [direct download](https://getintopc.com/softwares/3d-cad/solidworks-premium-2020-free-download-4526391/)
   
2. Check .NET Framework 3.5 and 4.0 are installed. If
   .NET Framework 3.5 (including 2.0) is not installed, go to 
   "Control Panel" -> "Programs and Features" -> "Turn Windows features on or off" ->
   -> select ".NET Framework 3.5 (including 2.0)"   

3.  Uninstall (if exist) SolidWorks_Flexnet_Server from SW2019 SSQ's release!
    To do it run as Administrator SolidWorks_Flexnet_Server\server_remove.bat 
    and wait until service "SolidWorks Flexnet Server" will be removed
    After that delete SolidWorks_Flexnet_Server folder from computer 
    1. Solidworks Flexnet Server doesn't exist.

4. Run "sw2020_network_serials_licensing.reg" and confirm to add info 
   into Windows Registry
   1. **Note, if not done properly, i can still delete this from regedit later.**

5. Copy folder "SolidWorks_Flexnet_Server" to C: , run as Administrator
   "SolidWorks_Flexnet_Server\server_install.bat" and wait until new service 
   "SolidWorks Flexnet Server" will be install and started

6.  Before installation, block the outgoing Internet access by means of Windows 
   Firewall or cord plug. 
   1. In Windows Defender Firewall with Advanced Security > Windows Defender Firewall Properties, block outbound for all profiles
      1. https://www.ghacks.net/2016/05/02/block-all-outbound-traffic-in-windows-firewall/ 
   2. I should do the install .NET Framework 3.5 first before blocking traffic.

7. Install SolidWorks 2020 (including PDM Client if required). 
   DO NOT install SolidNetwork License Server (SNL)!
   When asked of License Server definition input: 25734@localhost
   2. Don't reboot
   3. install on this computer
      1. Dont install SNL!
   4. No internet, press cancel, it will just install offline. good.
   5. Solidworks Electrical will try to connect to `localhost/TEW_SQLEXPRESS`. I have deleted the file from the previous installation. The service still tries to look for it, I have also deleted all the files from the regedit. 
      1. **So i just ask it to use a new server instance `<new instance name>/TEW`**
   
   ## exception handling

   6. If the System Check Warning window appears, ignore it (click Next to continue)
   
   7. If the warning "SolidWorks Serial number was not found in activation database" appears, ignore it (click OK to continue)
   
   8. If the full list of SW products to install is not visible, click "Select different package" and tick option "Select products not included in this package". Then select SW products to be installed

   9. If the "The Installation Manager was unable to determine the current subscription expiration date. Would you like to reactivate your license to update this information?" appears, press **No**. "Do you want to do it later?" prompt, press yes.
       

8. After end of setup overwrite original SolidWorks 2020 program folders (if exist)
   with cracked ones from folder "Program Files\SOLIDWORKS Corp" and "Program Files (x86)"

   Folders to be replaced from "Program Files\SOLIDWORKS Corp" (at setup by default):

   ```java
   C:\Program Files\SOLIDWORKS Corp\eDrawings  
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS CAM
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS Composer
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS Electrical
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS Explorer
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS Flow Simulation
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS Inspection
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS Manage Client
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS PCB
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS PDM
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS Plastics
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS Visualize
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS Visualize Boost
   ```

   Folders to be replaced from "Program Files (x86)" (at setup by default):

   ```java
   C:\Program Files (x86)\SOLIDWORKS PDM
   ```

   1. Services/tasks that i need to end first before deleting solidworks programfiles
      1. sw_fs
      2. dispatcher.exe (for flow simulation)
         1. I can't delete it either so i just put it in desktop lol
      3. SolidWorks Flexnet Server
      4. Solidworks Licensing Service
      5. Flexnet Licensing Service
      6. Flexnet Licensing Service 64
      7. SWVisualise2020.BoostService
      8. SWVisualise2020.Queue.Server
      9.  SOLIDWORKS > HoopsPublish > resource > Font
         1.  Just went to control panel > fonts and deleted them from there.
             1.  For font families, you can "open in new window" and see where the source file is (so you kno its frm solidworks)   
         2.  If this doesn't work, just move all the undeletable files to another folder like Desktop, then copy the replacement files over.
             1.  After you run the edit Windows Registry step, the programs won't reference them anymore and you can properly delete them.

9.  Run "SolidSQUADLoaderEnabler.reg" and confirm to add info 
   into Windows Registry

11. REBOOT COMPUTER!

12. Run SolidWorks > Help > SolidNetWork License Manager > License Order (you can also find it as `SolidNetwork License Manager Client 2020`)

    1. Use the "Move Up" and "Move Down" buttons to position Premium products with the same name higher than Professional and Standard products

    2. Click "Apply" to save the settings

    3. Click "OK" to close the SolidNetWork License Manager

13. Enjoy

NOTE:

   Since SW2019 network licensing crack uses other serial numbers than the previous (SW2010-2018)
   versions then if you installed SW2020 on one same computer with SW2010-2018 you need to:
 
   For SW2017-2018 reactivate them by running the corresponding SSQ's SW2017-2018 Activator (run 
   SSQ's SW2017-2018 Activator, select proper SW verssion and click "Activate Licenses")

   For SW2010-2016 replace original SolidWorks 2010-2016 program folders (if exist)
   with cracked ones from folder "Program Files\SOLIDWORKS Corp" and "Program Files (x86)"

   Folders to be replaced from "Program Files\SOLIDWORKS Corp" (at setup by default):

   ```java
   C:\Program Files\SOLIDWORKS Corp\eDrawings  
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS CAM
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS Composer
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS Electrical
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS Explorer
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS Flow Simulation
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS Inspection
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS Manage Client
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS PCB
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS PDM
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS Plastics
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS Visualize
   C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS Visualize Boost
   ```

   Folders to be replaced from "Program Files (x86)" (at setup by default):

   ```java
   C:\Program Files (x86)\SOLIDWORKS PDM
   ```

# How to uninstall


