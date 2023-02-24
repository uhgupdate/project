List Drives CMD via WMIC/CMD:
============================

Step 1. Press Win + R keys to open the Run dialog box, and then type cmd in it and press Ctrl + Shift + Enter keys together to open the elevated Command Prompt window.

Step 2. To let CMD list drives, type one of the following commands and hit Enter.

##wmic logicaldisk get name
##wmic logicaldisk get caption

Step 3. If you want to display the Device ID and volume name, type the following command and hit Enter. Also, you can run the fsutil fsinfo drives command to list drives on your computer

##wmic logicaldisk get deviceid, volumename, description

List Drives CMD via Diskpart:
============================

DiskPart is a disk partition management tool that uses command lines to perform operations. It can be used to list drives CMD as well. Here’s how to use it.

Step 1. Open the Command Prompt window again as we explained above.

Step 2. Type the following commands in order and hit Enter after each one. Then you will see a list of drives on the disk, including partition/volume number, label, letter, file system, size, and status.

##diskpart
##list disk
##select disk *
##list volume/list partition

How to List Drives in PowerShell:
================================

PowerShell is a command-line tool like CMD. Here you can let PowerShell list drives as well. To do so, follow the steps below:

Step 1. Open the Run dialog box, and then type powershell in it and hit Enter.

Step 2. In the Windows PowerShell window, type the following command and hit Enter.

##get-psdrive -psprovider filesystem

How to let PowerShell/CMD list drive letters? Now, I believe that you already have known the answer.
