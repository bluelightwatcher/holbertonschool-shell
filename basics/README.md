In this README you'll find a brief descriptions of the scripts.

First of all, the scripts needs to be 2 lines exactly.
All the scripts needs to end with en empty line.
The first line will always start with a shebang in order to "call the bash builtin function"
The second line will be the code itself
In order to create an empty I initially though of using this symbol /n, it is not necessary 

0-current_working_directory
runs pwd

1-listit
runs ls

2-bring_me_home
runs cd ~
the executable did not work in the terminal when running ./2-bring_me_home but it worked for the checker

3-listfiles
runs ls -l to display the long format

4-listmorefiles
runs ls -a -l
will display files in long format and hidden files

5-listmorefiles
runs ls -a -l -n
will display files in long format and hidden files plus the user ID and GID will be numbers
for instance my username etienne is replaced by 1000.

6-firstdirectory
runs mkdir /tmp/my_first_directory
Creates a directory with the absolute path

7-movethatfile
runs mv with origin path to destination/target path

8-firstdelete
runs rm /tmp/my_first_directory/betty
Will remove the file betty located in the /tmp/my_first_directory

9-firstdeletion
runs rmdir 
Removes empty directory.
If directory is not empty I would have to use the option -r (recursive) in order to remove the directory and the files within it

10-back
runs cd -
Changes the current directory to the previous one the user visited, different from the parent directory it can be in another branch of the file system

11-lists
runs ls -la . .. /boot
Option l stands for long format 
Option a stands for all 
. stands for current directory
.. stands for parent directory
/boot is the /boot directory
It prints files and hidden files in a long format

14-copy_html
runs cp -u wildcard.html .. 
The u option stands for update and will only overwrite existing file (ending with extension .html) with a newer version

15-lets_move
runs mv [[:upper:]](*) /tmp/u
Uses character class uppercase to move files starting by a capital letter to the /tmp/u file

16-clean_emacs
rm *~ 
This will remove all the file in the current directory ending with the ~extension (tilde) 

17-three
mkdir -p welcome/to/school
Option p stands for parent
This will create the directory school and all the parent directories specified in the path if need be

End of the shell basics 
