# Permission-File

File permission flowchart and apply the chmod command in a Python file to make the permissions rwxrwxr-x in linux terminal

File permission flowchart :
The flowchart serves as a visual representation of how access control works within a 
system. It clarifies how ownership and group membership influence what actions users 
can perform on a resource. By following the decision pathways, one can easily understand 
the hierarchy and rules governing access permissions.

terminal command :

At the beginning I start by opening a terminal window. Once the terminal is open, I create 
python file by write nano following by name of file , once click enter it will open file and 
know write code to change permission type .. then exit the file and write python3 following 
by name of file to run file then use the ls command, which will display the names of all files, 
including Python files that modified to permission (-rwxrwxr-x) .

python file (change_perFile):

The Python script code that changes the file permissions of a specified file using the os module. First, it imports the os module, which provides a way to interact with the operating system. The file_path variable is assigned the python file name . The os.chmod function is then called with two arguments: the file_path and the octal value 0o775. This octal value corresponds to the permissions rwxrwxr-x, meaning that the owner and group have read, write, and execute permissions, while others have read and execute permissions. By executing this script, the specified file's permissions will be updated accordingly, allowing for more flexible access control based on the specified permission settings.
