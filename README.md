# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

Name: K Vijay

Regno:212223040236
# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 
# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.
## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\MyLab
![image](https://github.com/vijaygowdu/Windows-basic-commands-batchscript/assets/147473788/528a3189-2594-433f-b9f8-d4f3ff03510a)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab
![image](https://github.com/vijaygowdu/Windows-basic-commands-batchscript/assets/147473788/f4261fea-d2ce-4e9f-a081-1d3afeeaf6c0)

![image](https://github.com/vijaygowdu/Windows-basic-commands-batchscript/assets/147473788/add459fe-4274-4007-ae28-86da5f0aa09e)

List the contents of the "MyLab" directory.
## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab
![image](https://github.com/vijaygowdu/Windows-basic-commands-batchscript/assets/147473788/d61a108d-87c5-43ec-990e-4c1eccf64faf)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
![image](https://github.com/vijaygowdu/Windows-basic-commands-batchscript/assets/147473788/453c834a-b6ee-48b5-9472-4ed7877d6c24)

![image](https://github.com/vijaygowdu/Windows-basic-commands-batchscript/assets/147473788/4c545975-081b-4b54-8d3e-e14b66c37930)

Move the "MyLab" directory to the "Documents" folder.
## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents
![image](https://github.com/vijaygowdu/Windows-basic-commands-batchscript/assets/147473788/10c715c8-e70a-454c-aab3-3dffe411996b)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT
![image](https://github.com/vijaygowdu/Windows-basic-commands-batchscript/assets/147473788/9566484b-09ef-4248-8f21-e18833ab98de)
# RESULT:
The commands/batch files are executed successfully.

