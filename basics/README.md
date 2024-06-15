In this README you'll find a brief descriptions of the scripts.

First of all, the scripts needs to be 2 lines exactly.
All the scripts needs to end with en empty line.
The first line will always start with a shebang in order to "call the bash builtin function"
The second line will be the code itself
In order to create an empty I initially though of using this symbol /n, it is not necessary 

The first script: 0-current_working_directory
runs pwd

The second script: 1-listit
runs ls

The third script: 2-bring_me_home
runs cd ~
the executable did not work in the terminal when running ./2-bring_me_home but it worked for the checker

The fourth script: 3-listfiles
runs ls -l to display the long format

The fifth script: 4-listmorefiles
runs ls -a -l
will display files in long format and hidden files

The sixth script: 5-listmorefiles
runs ls -a -l -n
will display files in long format and hidden files plus the user ID and GID will be numbers
for instance my username etienne is replaced by 1000.

The seventh script: 6-firstdirectory
runs mkdir /tmp/my_first_directory
create a directory with the absolute path

The eighth script: 8-movethatfile
runs mv with origin path to destination/target path

The ninth script : 9-firstdeletion
runs rmdir to remove empty directory if directory is not empty I would have to use the option -r (recursive) in order to remove the the directory and the files within it

The tenth script : 10-back
runs cd - which change the current directory to the previous one the user visited. different from the parent directory it can be in another branch of the file system

11-lists
runs ls -la . .. /boot
option l stands for long format 
option a stands for all 
. stands for current directory
.. stands for parent directory
/boot will list files in the /boot directory
it prints files and hidden files in a long format

14-copy_html
runs cp -u wildcard.html .. 
the u option stands for update and will only overwrite existing file (ending with extension .html) with a newer version

15-lets_move
runs mv [[:upper:]](*) /tmp/u
uses character class uppercase to move files starting by a capital letter to the /tmp/u file

16-clean_emacs
rm *~ 
this will remove all the file in the current directory ending with the ~extension (tilde) 

17-three
mkdir -p welcome/to/school
option p stands for parent
this will create the directory school and all the parent directories specified in the path if need be

End of the shell basics 
