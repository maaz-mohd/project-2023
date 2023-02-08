# Day6:File Permissions and Access Control Lists

### **#90DaysofDevops challenge**

### **File Permissions:**

In Linux, there are three types of owners for a file.

User - The user permissions apply only to the owner of the file or directory, they will not impact the actions of other users. user can also be called the default owner of the file.

Group - It is a collection of users. If you assign certain permission to a group same permission will be shared by all the members of the group.

Others - Any user that is not an owner of the file or doesn’t belong to the group can be categorized as others.

Linux file permissions for all three categories of users:  
i) `Read permission (r=4)` : It allows users to open and read the file only.  
ii) `` Write permission (w=2) ` ``: It allows the user to modify the file.  
iii) `Executable permission (x=1)` : It allows the user to run an executable script.

![No alt text provided for this image](https://media.licdn.com/dms/image/D4D12AQEalcgbZdWtHw/article-inline_image-shrink_1500_2232/0/1673179988765?e=1681344000&v=beta&t=SYce0IwSLeUe81YHRLTI0mNcNx4XdXF7MIXv7d_SMGI align="left")

we can find permissions of files and folders using a long listing **<mark>(ls -ltr)</mark>** on a Linux terminal.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1673373580241/122a60c2-2e53-4d1b-a5e4-dcf65fca6a6f.png?auto=compress,format&format=webp align="left")

In the output above, **<mark>d</mark>** represents a directory and **<mark>-</mark>** represents a regular file.

The **<mark>chmod</mark>** command enables you to change the permissions on a file.

### **Syntax of chmod:**

**chmod permissions filename**

Permissions can be changed using two modes:  
i)Symbolic mode  
ii)Absolute mode

**Symbolic mode:**

The permissions for a file or directory can be set for the owner, for the group that the file belongs to, and for all other users. The “**u**”, “**g**”, and “**o**” options stand for the user, group, and others, respectively. The “**+**” and “**\-**” signs are used to add and remove permissions, respectively. The “**x**” permission allows a file to be executed. The “**w**” permission allows a file to be modified. The “**r**” permission allows a file to be read or a directory to be listed.

<mark>Ex: chmod u+x file.txt</mark>

chmod o-r file.txt

**Absolute mode:**

In absolute mode we have to use numbers to assign permissions.

Ex: chmod 777 file.txt

**<mark>chgrp</mark>** command is used to change the group ownership of the file or directory.

### Read about ACL and try out the commands `getfacl` and `setfacl`

The “**getfacl**” and “**setfacl**” commands are used to get and set file access control lists (ACLs) in Linux. ACLs allow you to specify fine-grained permissions for files and directories beyond the standard user, group, and other permissions.

**i)If ACL is not enabled in our file system**

Command to install acl: sudo apt install acl.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1673375512007/4e314f99-4c69-4908-ae22-1370820105cd.png?auto=compress,format&format=webp align="left")

**ii)getfacl**

The output of the “**getfacl**” command will show the ACLs for the file, including the owner, group, and permissions for each user and group.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1673375612975/b6ac824a-c85c-49d1-a0ad-6a94d1b20c3e.png?auto=compress,format&format=webp align="left")

**iii)setfacl**

“**setfacl**” is used to set or modify the ACLs of a file or directory.

For example, to give read and execute permissions to “user2" and read permission to “user3” for a file called “myfile” you would run

**setfacl -m u:user2:rx,u:user3:r myfile**

The “**\-m**” option tells “**setfacl**” to modify the existing ACLs of the file. The “**u:user2:rx**” and “**u:user3:r**” values specify the permissions to set for “**user2**” and “**user3**" respectively.

**Thanks for reading! Happy Learning!!**