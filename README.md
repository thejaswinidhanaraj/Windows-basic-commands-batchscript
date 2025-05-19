# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file . Save each script in a file with a .bat extension. Ensure you have the necessary permissions to perform the operations. Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "my-folder"

## COMMAND AND OUTPUT
```
Create a directory named "MyLab" on the desktop.
```
![Screenshot 2025-05-15 152331](https://github.com/user-attachments/assets/ec2aec5b-5b5b-413b-8bb3-76440de849be)
Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-15 152341](https://github.com/user-attachments/assets/4dd56e68-27be-4f9b-a738-af112f57b8d0)
```
type nul > MyFile.txt
```
![Screenshot 2025-05-15 152351](https://github.com/user-attachments/assets/bddb2b95-2990-47ad-afb0-e1f4451225da)
List the contents of the "MyLab" directory.
## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-15 152402](https://github.com/user-attachments/assets/c44d3fc1-c31a-42fc-b6c3-0a1b9f1bf27a)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```
![Screenshot 2025-05-15 152429](https://github.com/user-attachments/assets/475e48b1-cf04-43e4-a10a-9d580e3d1b50)

```
copy MyFile.txt %userprofile%\Desktop\Backup
```
Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
```
![Screenshot 2025-05-15 152447](https://github.com/user-attachments/assets/52d38d25-8a7c-4e02-8564-87cd26083f24)

## Exercise 2: Advanced Batch Scripting
Create a batch file named on the desktop. The batch file need to have a variable assigned with a desired name for ex. name="John" and display as "Hello, John".

## COMMAND AND OUTPUT
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
![Screenshot 2025-05-15 152458](https://github.com/user-attachments/assets/d9f6a6d9-8bf3-4d4a-a7af-4998b91193c6)


## COMMAND AND OUTPUT
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
![Screenshot 2025-05-15 152510](https://github.com/user-attachments/assets/4c2e2c93-47b9-4db1-8c7f-b3cbb911608a)

# RESULT:
The commands/batch files are executed successfully.

