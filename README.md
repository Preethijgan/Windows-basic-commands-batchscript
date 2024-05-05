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
![Screenshot 2024-05-05 180203](https://github.com/Preethijgan/Windows-basic-commands-batchscript/assets/144870652/80cb2424-a260-4f56-bfcf-58e533d4497b)




## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab

```
![Screenshot 2024-05-05 180302](https://github.com/Preethijgan/Windows-basic-commands-batchscript/assets/144870652/9a8501d1-b220-422e-980f-a76bdb5c8396)
![Screenshot 2024-05-05 180337](https://github.com/Preethijgan/Windows-basic-commands-batchscript/assets/144870652/9224d7fb-a4fd-4a1e-a1a4-2433722875c1)





## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab

```
![Screenshot 2024-05-05 180637](https://github.com/Preethijgan/Windows-basic-commands-batchscript/assets/144870652/01529418-e0dc-44ca-90ef-a3ce4ba33578)



## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.

```
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
```
![Screenshot 2024-05-05 180810](https://github.com/Preethijgan/Windows-basic-commands-batchscript/assets/144870652/a0dbb303-e603-4a48-b308-ccaeb318e56e)



## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![Screenshot 2024-05-05 180922](https://github.com/Preethijgan/Windows-basic-commands-batchscript/assets/144870652/eb1d3916-8346-4456-b72f-f8201d23fa16)



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

![Screenshot 2024-05-05 181132](https://github.com/Preethijgan/Windows-basic-commands-batchscript/assets/144870652/524e0614-396d-49f2-8992-0135b4bcf177)




# RESULT:
The commands/batch files are executed successfully.

