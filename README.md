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

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

```
mkdir %userprofile%\Desktop\MyLab
```

![Screenshot 2024-05-06 160409](https://github.com/syedfayaz3105/Windows-basic-commands-batchscript/assets/144870652/e645a0cf-c15e-4878-9198-0bfe3545d262)



## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![Screenshot 2024-05-06 160509](https://github.com/syedfayaz3105/Windows-basic-commands-batchscript/assets/144870652/7ba1f914-b9f9-4465-afff-5070ab1b76f2)
![Screenshot 2024-05-06 160537](https://github.com/syedfayaz3105/Windows-basic-commands-batchscript/assets/144870652/489ee6b2-55dc-4b2c-a491-1ba582253bed)




## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![Screenshot 2024-05-06 160622](https://github.com/syedfayaz3105/Windows-basic-commands-batchscript/assets/144870652/3ecabfe2-06c0-4429-83eb-c6efcf8c8000)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
```
![Screenshot 2024-05-06 160704](https://github.com/syedfayaz3105/Windows-basic-commands-batchscript/assets/144870652/47f9ae3f-7832-41e8-9e1e-b70b9a9d992a)



## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![Screenshot 2024-05-06 160748](https://github.com/syedfayaz3105/Windows-basic-commands-batchscript/assets/144870652/8ca09d49-c643-4a09-8db6-d3b52d9231de)



## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT

![Screenshot 2024-05-06 160946](https://github.com/syedfayaz3105/Windows-basic-commands-batchscript/assets/144870652/2162366e-2e03-4754-982a-81ae59d67170)




# RESULT:
The commands/batch files are executed successfully.

