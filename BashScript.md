# bashScript
Contains bash script files for beginers

-   echo : Works like print statement to print something on the terminal

    -   To forget or not using new line character by default you have to use 

            echo -n "second line"
    -   To allow special character to work use
            echo -e "\nSpecial character"


-   To set multi line comment

    -   Colon [:] Should be present at starting after ward put all comment in single quotes

            : 'put all data like this'


-   To do mathematical work type like this

        ((result=$num/17))

-   To print mathematical output inside the echo type:
    -   After echo give a pipe and type "bc"
       
             echo $num/17 | bc

-   To get decimal value put -l afterwards

        echo $num/17 | bc -l

-   To concat the two string variable

        result="$var1 $var2"      

-   To get the substring from the whole string

         str="hey World"
         subString=${str:0:2}

         # 0 here is the starting position
         # 2 is the number of characters

-   Checking multiple if condition:

         if [[ ($var -le 0  && $rand -eq 5) ]];

         # If you put || in place of && it will work as OR command 


-   To get several arguments from command line:
   -   [$#] : Used to set multiple arguments


            args=$#
             var=$1
             var2=$2
-   Until Loop is different from while:
   -   Until loop will run till the condition become false. On the other side while will run till the condition become false


-   Calling function which return some value
         
         AddReturn()
         {
             ((out=$1+$2))
             echo "inside the loop"
             echo $out
            }

        # calling the function here
         
         valOutput=$(AddReturn 10 2)
         echo $valOutput



-   We have two type of environment variable
   -   Shell variable
   -   Environment variable

            export name="value"

            [Will only be present locally mean for that terminal only]

   -   export name="val"
         -   [Put that in ~/.bashrc file to make it permanent]



-   Alias : It is used to set the small name to everthing. Save this permananetly to .bashrc file

         alias name="cd /home/tushar/Desktop"


-   Wildcards: Are used to ease your work

         cp {*.mp3,*mp4} /destination

-   Run multiple command 
   -   This will run the command as random
           
           cp ; ls ; pwd

   -   To run the command in sequence what need to what to get it complete use:

           cp && pwd && ls




