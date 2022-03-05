# Week 2 Lab Report 

    This post is about how I set up ieng6 account. 

    Author:Guidong Luo

---
* **Step 1**\
Installing VS Code(or other code editors)

    ![Image](Images\vscode.png)

     I already set up vs code in last quarter when taking CSE 11, so I can't show you how to install it, but you can easily download it at [Visual Studio Code](https://code.visualstudio.com/).
* **Step 2**\
Remote Connecting

    ![Image](Images\connect.png)
Before doing this,I first changed my password through [Account Lookup](https://sdacs.ucsd.edu/~icc/index.php).

    *It actually took me lots of efforts to set it up*:(
    
    After that, I opened the termianl and typed in
    >ssh cs15lwi22avn@ieng6.ucsd.edu> 

    Then I was able to enter the password and successfuly connect to the server.
* **Step 3**\
Runing Commands


     ![Image](Images\c2.png)
     >ls

    ![Image](Images\command.png)
    >ls -a

     ![Image](Images\c3.png)
     >run java files

* **Step 4**\
Moving Files with scp


    ![Image](Images\copy.png)
    >scp path account\
    (I already set up SSH key, so here I don't need to type in the password.)

* **Step 5**\
Settting an SSH Key


    ![Image](Images\key.png)
    > First, generate the key here

    (Then we need to enter mkdir .ssh in the server)
    ![Image](Images\key2.png)
    > Add pub key to the server
* **Step 6**\
Optimizing Remote Running

    1\.

   ![Image](Images\o1.png)
   >Use "" to directly run the command 

   It only take us 1 keystroke to show all the files in the server. For comparison, we can see that we need to take 2 keystrokes before. This saves us 1 keystroke.

    ![Image](Images\com1.png)

    2\.

   ![Image](Images\o2.png)
   > Use semicolons to run multiple commands at the same time


   Combining these two strategies, we can remotely run a program using 1 keystroke
   ![Image](Images\com2.png)

   While the traditional way needs 3 keystrokes
   ![Image](Images\com3.png)
