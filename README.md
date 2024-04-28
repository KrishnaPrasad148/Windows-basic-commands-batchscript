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

### 1) Create a directory named "MyLab" on the desktop.

#### COMMAND AND OUTPUT:
```
mkdir %userprofile%\Desktop\MyLab
```
![Screenshot 2024-04-28 100248](https://github.com/KrishnaPrasad148/Windows-basic-commands-batchscript/assets/147332763/7ac7df08-c3c9-447d-9b72-6e61bac7f8b2)




### 2) Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

#### COMMAND AND OUTPUT:
```
cd %userprofile%\Desktop\MyLab
type nul > MyFile.txt
```
![Screenshot 2024-04-28 123935](https://github.com/KrishnaPrasad148/Windows-basic-commands-batchscript/assets/147332763/ab3de74c-3482-4a9e-ae5a-1a42052c120d)



### 3) List the contents of the "MyLab" directory.

#### COMMAND AND OUTPUT:
```
dir %userprofile%\Desktop\MyLab
```
![Screenshot 2024-04-28 124242](https://github.com/KrishnaPrasad148/Windows-basic-commands-batchscript/assets/147332763/db165efa-79e8-4293-807e-9ff343471d12)



### 4) Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

#### COMMAND AND OUTPUT:
```
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
```
![Screenshot 2024-04-28 124452](https://github.com/KrishnaPrasad148/Windows-basic-commands-batchscript/assets/147332763/4ce4ebad-a01c-47fa-824d-b0c9e30d2dc5)



### 5) Move the "MyLab" directory to the "Documents" folder.

#### COMMAND AND OUTPUT:
```
move %userprofile%\Desktop\MyLab  %userprofile%\Documents
```
![Screenshot 2024-04-28 124846](https://github.com/KrishnaPrasad148/Windows-basic-commands-batchscript/assets/147332763/812d4de2-63d9-44be-8bc4-be09f0722e7a)



## Exercise 2: Advanced Batch Scripting
### Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!

```
### Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!

```




## OUTPUT

![Screenshot 2024-04-28 130146](https://github.com/KrishnaPrasad148/Windows-basic-commands-batchscript/assets/147332763/5cc1d37a-6752-4668-bfeb-70a28c4bc12a)

![Screenshot 2024-04-28 130313](https://github.com/KrishnaPrasad148/Windows-basic-commands-batchscript/assets/147332763/75a13224-ba19-48d8-92c6-d4b1c6ea43ad)




# RESULT:
The commands/batch files are executed successfully.

