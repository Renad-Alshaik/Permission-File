# Permission-File
# Descreption about permission File
In Linux, every file and directory has a set of permissions that control who can access and modify it. These permissions determine what actions a user can perform on a file or directory, such as reading, writing, or executing it. The permissions are divided into three categories: owner, group, and others. The owner is the user who created the file, the group consists of users who belong to the same group as the file, and others refers to everyone else.
Each category can have three types of permissions: read (r), write (w), and execute (x). The read permission allows a user to view the contents of a file, the write permission allows modifying the file, and the execute permission allows running the file as a program or script. Permissions are represented by a combination of these letters. For example, rwxrwxr-x means that the owner and group have full permissions (read, write, and execute), while others have only read and execute permissions.
Permissions are also represented numerically using an octal system. In this system, each permission type has a corresponding number: read is 4, write is 2, and execute is 1. These values are added together to represent different combinations of permissions. For example, rwx is equivalent to 7 (4 + 2 + 1), while rw- is 6 (4 + 2). To set file permissions using the numeric system, you can use the chmod command followed by the permission value. For instance, chmod 775 file.txt sets the permissions to rwxrwxr-x, giving the owner and group full permissions and others read and execute permissions.
The first character in the output of the ls -l command indicates the type of file. A dash (-) represents a regular file, while a d represents a directory. Other symbols include l for symbolic links, c for character devices, and b for block devices.
# Task
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
