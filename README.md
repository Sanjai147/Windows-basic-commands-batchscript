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
mkdir %userprofile%\Desktop\MyLab
![image](https://github.com/Sanjai147/Windows-basic-commands-batchscript/assets/162275632/be700ea3-eb40-47cc-b043-2e51a9f0d3a4)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab
![image](https://github.com/Sanjai147/Windows-basic-commands-batchscript/assets/162275632/4eb503c7-c9b6-4168-bbb2-507801311a01)
![image](https://github.com/Sanjai147/Windows-basic-commands-batchscript/assets/162275632/b2b023cf-763e-4da6-aad1-2d2b3ffa0b26)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab
![image](https://github.com/Sanjai147/Windows-basic-commands-batchscript/assets/162275632/873b3d3f-8feb-4817-a1ae-8c69090c8674)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
![image](https://github.com/Sanjai147/Windows-basic-commands-batchscript/assets/162275632/0392c502-c5c2-4314-8fb6-541d40c618df)

![image](https://github.com/Sanjai147/Windows-basic-commands-batchscript/assets/162275632/debef933-adc0-4991-86f6-20584a993045)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT

mv Myfile.txt %userprofile%\Documents
![image](https://github.com/Sanjai147/Windows-basic-commands-batchscript/assets/162275632/c8a8d351-d483-4653-ba46-f3423e43112b)


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
![image](https://github.com/Sanjai147/Windows-basic-commands-batchscript/assets/162275632/372af71e-6ab0-4ff6-bf2d-c3a3aa4e7c1e)




# RESULT:
The commands/batch files are executed successfully.

