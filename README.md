# Permission-File
# apply the chmod command in a Python file to make the permissions rwxrwxr-x in linux terminal

# << terminal command >>

renad@Renad:~$ ls
Desktop  Documents  Downloads  Music  Pictures  Public  Templates  Videos
renad@Renad:~$ nano change_perFile.py
renad@Renad:~$ ls -l
total 36
-rw-rw-r-- 1 renad renad   95 يناير   6 14:52 change_perFile.py
drwxr-xr-x 2 renad renad 4096 ديسمبر 31 18:15 Desktop
drwxr-xr-x 2 renad renad 4096 ديسمبر 31 18:15 Documents
drwxr-xr-x 2 renad renad 4096 ديسمبر 31 18:15 Downloads
drwxr-xr-x 2 renad renad 4096 ديسمبر 31 18:15 Music
drwxr-xr-x 2 renad renad 4096 يناير   5 00:10 Pictures
drwxr-xr-x 2 renad renad 4096 ديسمبر 31 18:15 Public
drwxr-xr-x 2 renad renad 4096 ديسمبر 31 18:15 Templates
drwxr-xr-x 2 renad renad 4096 ديسمبر 31 18:15 Videos
renad@Renad:~$ cd /home/renad
renad@Renad:~$ python3 change_perFile.py
permissions change
renad@Renad:~$ ls
change_perFile.py  Documents  Music     Public     Videos
Desktop            Downloads  Pictures  Templates
renad@Renad:~$ ls -l
total 36
-rwxrwxr-x 1 renad renad   95 يناير   6 14:52 change_perFile.py
drwxr-xr-x 2 renad renad 4096 ديسمبر 31 18:15 Desktop
drwxr-xr-x 2 renad renad 4096 ديسمبر 31 18:15 Documents
drwxr-xr-x 2 renad renad 4096 ديسمبر 31 18:15 Downloads
drwxr-xr-x 2 renad renad 4096 ديسمبر 31 18:15 Music
drwxr-xr-x 2 renad renad 4096 يناير   5 00:10 Pictures
drwxr-xr-x 2 renad renad 4096 ديسمبر 31 18:15 Public
drwxr-xr-x 2 renad renad 4096 ديسمبر 31 18:15 Templates
drwxr-xr-x 2 renad renad 4096 ديسمبر 31 18:15 Videos

# << code of python file >>
import os
file_path ='change_perFile.py'
os.chmod(file_path,0o775)
print("permissions change")

Description:  
At the beginning I start by opening a terminal window. Once the terminal is open, I create 
python file by write nano following by name of file , once click enter it will open file and 
know write code to change permission type .. then exit the file and write python3 following 
by name of file to run file then use the ls command, which will display the names of all files, 
including Python files that modified to permission (-rwxrwxr-x) .
