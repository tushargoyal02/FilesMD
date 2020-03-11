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



