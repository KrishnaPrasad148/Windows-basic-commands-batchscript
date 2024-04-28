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
![image](https://github.com/KrishnaPrasad148/Windows-basic-commands-batchscript/assets/147332763/185e13d8-30aa-41cb-b892-6663192780a6)



### 2) Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

#### COMMAND AND OUTPUT:
```
cd %userprofile%\Desktop\MyLab
type nul > MyFile.txt

```



### 3) List the contents of the "MyLab" directory.

#### COMMAND AND OUTPUT:
```
dir %userprofile%\Desktop\MyLab
```


### 4) Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

#### COMMAND AND OUTPUT:
```
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
```


### 5) Move the "MyLab" directory to the "Documents" folder.

#### COMMAND AND OUTPUT:
```

```


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





# RESULT:
The commands/batch files are executed successfully.

