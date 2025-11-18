# EX 6: MOVING FILES BETWEEN VIRTUAL MACHINES

### NAME: VISWAJITH LALITHRAM R.V
### REG NO: 212224240187

## Aim:
To move the files between virtual machine.
 You can move files between virtual machines in several ways:
•	You can copy files using network utilities as you would between physical computers on your network. To do this between two virtual machine:
•	Both virtual machines must be configured to allow access to your network.
•	Any of the networking methods (host-only, bridged and NAT) are appropriate. 
•	With host-only networking, you copy files from the virtual machines to the host and vice-versa, since host-only networking only allows the virtual machines see your host computer.
•	With bridged networking or NAT enabled, you can copy files across your network between the virtual machines.
•	You can create a shared drive, either a virtual disk or a raw partition, and mount the drive in each of the virtual machines.
## Procedure:
### How to Enable File sharing in VirtualBox. 
Step 1. Install Guest Additions on the Guest machine. 
Step 2. Configure File Sharing on VirtualBox. 
 
Step 1. Install Guest Additions on the Guest machine. 
1. Start the Virtuabox Guest Machine (OS). 
2. From Oracle's VM VirtualBox main menu, select Devices > Install Guest Additions *

a. Open Windows Explorer
b. Double click at the "CD Drive (X:) VirtualBox Guest additions" to explore its contents.
		  
<img width="922" height="745" alt="1" src="https://github.com/user-attachments/assets/f9a4f8b0-3c07-4b90-a197-d50528ec87a5" />


C.Right click at "VBoxWindowsAdditions" application and from the pop-up menu, choose "Run as administrator".
 
<img width="986" height="471" alt="2" src="https://github.com/user-attachments/assets/3bd4187c-bc28-4c7d-b3c9-04bdce937bf5" />


3.Press Next and then follow the on screen instructions to complete the Guest Additions installation.
	 
<img width="965" height="636" alt="3" src="https://github.com/user-attachments/assets/4f1dc00d-e650-4389-926d-f5125e785987" />


4. When the setup is completed, choose Finish and restart the Virtuabox guest machine.
Step 2. Setup File Sharing on VirtualBox Guest Machine.
1. From VirtualBox menu click Devices and choose Shared Folders -> Shared Folder Settings.

<img width="1057" height="625" alt="4" src="https://github.com/user-attachments/assets/50f31b9e-dcaf-49bc-8cd3-47f04e44dc63" />


2. Click the Add new shared folder icon.
   
<img width="1057" height="625" alt="5" src="https://github.com/user-attachments/assets/8949bd22-31dc-4b8a-8f21-8ce39a914d53" />



4. Click the drop-down arrow and select Other.
 
<img width="1100" height="757" alt="6" src="https://github.com/user-attachments/assets/8e78c8f2-0c96-41c5-a1c7-2fa95105ee9e" />


3. Locate and highlight (from the Host OS) the folder that you want to share between the VirtualBox Guest machine and the Host and click Select Folder. *
* Note: To make your life easier, create a new folder for the file sharing, on the Host OS and give it with a recognizable name. (e.g. "Public")
 
<img width="1067" height="553" alt="7" src="https://github.com/user-attachments/assets/56287d0b-1a1c-4ea6-b900-35456c51ca0a" />


4. Now, in the 'Add Share' options, type a name (if you want) at the 'Folder Name box, click the Auto Mount and the Make Permanent checkboxes and click OK twice to close the Shared Folder Settings.
 
<img width="1035" height="516" alt="8" src="https://github.com/user-attachments/assets/d187fc07-3d5f-4f2e-a889-76100b25d58e" />


5. You 're done! To access the shared folder from the Guest OS, open Windows Explorer and under the 'Network locations' you should see a new network drive that corresponds to the shared folder on the Host OS.

## Result:

Thus the virtual machine files are moved to another VM.
