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
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/NIHITHARANI/Windows-basic-commands-batchscript/assets/149365740/7b8aaa29-e182-4030-b5a7-edf0dacc9a52)



## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/NIHITHARANI/Windows-basic-commands-batchscript/assets/149365740/37180126-a93b-44f0-9daf-a7a3068dd671)



![image](https://github.com/NIHITHARANI/Windows-basic-commands-batchscript/assets/149365740/8452701d-ae6f-4265-9288-1f3a044dfffa)


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/NIHITHARANI/Windows-basic-commands-batchscript/assets/149365740/d867d574-0555-4814-a892-17189133789c)



## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/NIHITHARANI/Windows-basic-commands-batchscript/assets/149365740/8f786807-92f9-478f-afc9-507f07e4d78a)



![image](https://github.com/NIHITHARANI/Windows-basic-commands-batchscript/assets/149365740/bf42a71c-e5a8-4542-897b-16c593a1c6e8)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mv Myfile.txt %userprofile%\Documents
```
![image](https://github.com/NIHITHARANI/Windows-basic-commands-batchscript/assets/149365740/cfea6ffb-df0b-483a-8e7d-49675f0921b4)




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

![image](https://github.com/NIHITHARANI/Windows-basic-commands-batchscript/assets/149365740/be935888-3134-41e4-ae32-d3a1fd86f10f)




# RESULT:
The commands/batch files are executed successfully.

