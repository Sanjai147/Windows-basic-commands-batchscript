# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

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
mkdir%userprofile%\Desktop\MyLab
![WhatsApp Image 2024-04-28 at 16 31 54_d61ec236](https://github.com/gowriganeshns/Windows-basic-commands-batchscript/assets/162275632/a97dd5f5-0b57-4e19-8577-6727840a55a5)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop/\MyLab
![WhatsApp Image 2024-04-28 at 16 32 34_a25233d7](https://github.com/gowriganeshns/Windows-basic-commands-batchscript/assets/162275632/7e6d0714-4956-4043-a201-c16189690d80)

![WhatsApp Image 2024-04-28 at 16 32 49_a8817109](https://github.com/gowriganeshns/Windows-basic-commands-batchscript/assets/162275632/de812c43-053c-4244-9c8c-ef751efb58fe)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab
![image](https://github.com/gowriganeshns/Windows-basic-commands-batchscript/assets/162275632/917f0cb5-aa61-4b84-a790-c2d3c2a5f7d4)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
![image](https://github.com/gowriganeshns/Windows-basic-commands-batchscript/assets/162275632/15eeebfe-b2d3-42ac-a14e-f1694ce82e3c)
![image](https://github.com/gowriganeshns/Windows-basic-commands-batchscript/assets/162275632/bc4c6a85-3e5b-4d28-b35f-d0c516d72be1)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents
![image](https://github.com/gowriganeshns/Windows-basic-commands-batchscript/assets/162275632/3fe7f92b-a948-432e-b7f2-2260e6244703)

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
![image](https://github.com/gowriganeshns/Windows-basic-commands-batchscript/assets/162275632/e49bee0a-94cb-4439-bae6-411b7ac1ea87)

# RESULT:
The commands/batch files are executed successfully.

