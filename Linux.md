##  Here we will talk about the linux commands

-   ls : list all items
    -   ls -l : detailed information
    -   ls .Do* : All files starting with Do
    -   ls .*  : all hidden files
    -   ls -a : Same as above show all hidden files

-   cd : Used to change the directory
    -   " cd  -  " : Move you to the previous directory in which you were in at that time

    -   " cd .. " : This will let you move to the previous directory only

### To maintain the history of files changes you can use pushd & popd . While dirs is used to show the history only

-   pushd '/path/target' : This will move you to new folder with history of all data

    -   It will show you where were you and now where you have moved

            dirs : To print all stack history

-   popd : This simple command will move back to the previous directory you have worked on like " cd  - "


-   To know what we contain in file like type of data or file format


        file "/filename"


-   To locate file with the data or some particular characters
        
        locate CHARACTERname
    -   If you don't receive any file from your computer as might be the database for file changes have not been done so far.

            sudo updatedb

-   Check where a command is saved in your computer type:

        which Command_Name


-   To know what is the particular function of a command

        whatis command_Name

-   Find out command where it is present.

        apropos Command_name

    -   It will search for the command name in all places also in description

-   Get detailed knowledge of a command

        man command_name

-   mkdir folder_name: To make a directory

-   touch file : To create empty file if doesn't exist


-   rm -r : Remove file recursively
-   rmdir : REmove empty directory

-   chmod : Changes the permission
           
         chmod 777 filename

   -   RWX permission are present R=4, w=2, x=1


-   cat >> file.txt
      -    this will allow what you type on terminal to save in that file
      -   It will append the data
      if the file is already there

            Press CTRL + D (to save and exit)

-   more fileName : Works as a page
      -   Show file as a page and in manageable format

-   less filename: More advanced of version of more

-   sudo : SUDO stands for superuser do
-   To move to sudo user

         sudo -s

-   To get all users present in your system
      
         users

-   To show the id's of any particular users use:

         id

-   killall chrome : This command will kill all instance of that application.

-   To see which process are running

           ps -ax


##   Shortcut Keys:


-   CTRL + A : This will move the cursor to the first word in terminal
-   CTRL + E: It will move to the last line of character in terminal

-   ALT + B : This will move you to the first character of the word

-   ALT + F : Will move forward to first character of the word



###   DELETE :
-   To delete all word to the right of cursor
   -   It basically cuts the line
      
            CTRL + K

- Let's say you have the command like this:
   -   "mv /home/tushar/Desktop"
   -   You want only "Desktop" and all the thing should be deleted

            CTRL + X [After this Press "BACKSPACE" ]


-   To undo the command what you have typed in terminal is:

        CTRL + Shift + _ 

-   If you want to interchange the character or word press:

        ALT + T


### COPY AND PASTE :
-   To cut something in terminal press:

        CTRL + W

-   To paste what you have cut is:
      
         CTRL + Y


###   To capitalize all the words

-   To capitalise the word from cursor is

         ALt + U

-   To uncapitalise it

         ALT + L


-   Only 1 character of the word on the cursor

         ALT + C




