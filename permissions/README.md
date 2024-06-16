Here we will list the requirements for each script followed by a brief description of each scripts

Allowed editors: vi, vim, emacs
All your scripts will be tested on Ubuntu 22.04 LTS
All your scripts should be exactly two lines long ($ wc -l file should print 2)
All your files should end with a new line (why?)
The first line of all your files should be exactly #!/bin/bash
A README.md file, at the root of the folder of the project, describing what each script is doing
You are not allowed to use backticks, &&, || or ;
All your files must be executable

0-i_am_betty
su betty 
switch current user to betty

1-who_am_i
id -un 
print user name

2-groups
id -nG
print name of users in the group

3-new_owner
chown betty hello
change owner of the file hello to betty

4-empty
touch hello
creates an empty file named hello

5-execute
chmod u+x hello
ads executable permission to the user on the file named hello

6-multiple_permissions
chmod 754 hello
gives rwx permissions to the user, rx permissions to the group, r permissions to other users on the file named hello

7-everybody
chmod ugo+x hello
adds executable permissions on the file named hello for all the users. 

if we just need to allow one type of permissions, it might be easier to use the ugoa format rather than the octal mode (775) because we would not mess up with the current state of permissions too much. 


8-James_Bond
chmod 007 hello
gives no permissions for the user, no permissions for the owning group, but read write and execute permissions to all the other users on the file named hello. 

9-john_Doe
chmod 753 hello
give all permissions to user, read and write permissions for the group and write and execute permissions for the other users, on the file named hello. 

10-mirror_permissions
chmod --reference=olleh hello
chmod attributes the same permissions of the olleh file to the hello file

11-directories_permissions
chmod -R a+x */
changes permissions by adding executable permissions to all users in a recurssive manner. Using wildcard with a forward slash to apply the changes only to directories and sub directories in the current directories. 

12-directory_permissions
mkdir -m 751 my_dir
creates the my_dir directory and changing the permissions using the -m option.  751 informs the computer to give rwx to user rx to group and execute to the other user

*keep in mind that for directories executing means beeing able to open the folder.* 

13-change_group
chgrp school hello
changes the group owner to school for the file hello

14-change_owner_and_group
chown vincet:staff *
change the owner to vincent and group owner to staff for all the file in the current directory due to the wildcard *

15-symbolic_link_permissions
chown -RP vincet:staff _hello
changes the owner and group of the _hello file. _hello beeing a symbolic link I used RP to not traverse the link and modify its permissions. the 

16-if_only
chown --from=guillaume vincent hello
changes the owner of the file hello to vincent  only if the owner is guillaume

