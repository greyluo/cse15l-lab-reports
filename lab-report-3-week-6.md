# Week 6 Lab Report 
    This is a post about Option 1
    Author: Guidong Luo

## **Introduction**

    Setting up ssh configuration on Windows is quite different from Linux.
    I will show you step by step how I settled it.
    

## **Step 1** Find the .ssh folder
 In Windows, we can't simply put use ~/.ssh/config and edit it. I first found this ./ssh folder and then opened it using Git Bash, which alllows me to use Linux command.


 ![Image](Images\lab3\ssh.png)
   
*(Click "Git Bash Here".Thank you, Git Bash!)*


## **Step 2** Create config file
I guess that config file is not a default file in .\ssh for windows. So, we need to create it on Git Bash command line.


![Image](Images\lab3\touch.png)


I used touch command to create config file because I don't know how to create a *File* otherwise.


## **Step 3** Set up config file
Open it using noteboook (so lame) and then copy&paste the commands from the lab notes. Change the user account to mine.


![Image](Images\lab3\edit.png)


## **Finally**
![Image](Images\lab3\result.png)


