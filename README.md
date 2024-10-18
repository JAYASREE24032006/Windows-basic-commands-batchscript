# EX8 - Windows-basic-commands-batchscript

## AIM :
To execute Windows basic commands and batch scripting

## DESIGN STEPS :

### Step 1 :

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2 :

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.

### Step 3 :

Execute the necessary commands/batch file for the desired output. 




## WINDOWS COMMANDS :
### Exercise 1 : Basic Directory and File Operations :


Create a directory named "MyLab" on the desktop.

#### COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\MyLab
```

![image](https://github.com/user-attachments/assets/fac0bb31-e04c-4b4c-be64-a5ec417e5ac4)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

#### COMMAND AND OUTPUT :

```
cd %userprofile%\Desktop\MyLab
```

![image](https://github.com/user-attachments/assets/051a7a82-4779-49a1-ac28-7e88c15e5d8a)

```
type nul > MyFile.txt
```

![image](https://github.com/user-attachments/assets/4d06c5bc-9dea-47e4-81db-1a267251df55)



List the contents of the "MyLab" directory.


#### COMMAND AND OUTPUT :

```
dir %userprofile%\Desktop\MyLab
```

![image](https://github.com/user-attachments/assets/f8743d2b-85b8-4640-b7a2-6d86bab94d9e)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

#### COMMAND AND OUTPUT :

```
mkdir %userprofile%\Desktop\Backup
```

![image](https://github.com/user-attachments/assets/ffe4f5d9-67dc-4d32-817d-ec5127c01f14)

```
copy MyFile.txt %userprofile%\Desktop\Backup
```

![image](https://github.com/user-attachments/assets/3422e300-3b98-4c51-a633-bf18941e6b9e)



Move the "MyLab" directory to the "Documents" folder.


#### COMMAND AND OUTPUT :

```
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
```

![image](https://github.com/user-attachments/assets/dd042c70-ed55-4cbd-bd3f-fbeacc324946)


### Exercise 2 : Advanced Batch Scripting :

Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

#### COMMAND AND OUTPUT :

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```



![image](https://github.com/user-attachments/assets/3a9ba2fc-710a-4d46-a436-28ee3d67eab6)




## RESULT :
The commands/batch files are executed successfully.

