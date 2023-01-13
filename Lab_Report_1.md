Lab Report 1
=========
Step 1: Installing Visual Studio Code

  Click the following link: https://code.visualstudio.com/
  It will take you to a page that looks like this: 
  <img width="1728" alt="Screen Shot 2023-01-12 at 4 54 39 PM" src="https://user-images.githubusercontent.com/122579715/212212419-9cb0ac92-9fd1-43ac-a47c-1f272fb88824.png">

  Click the download button at the top right of the page, which will prompt you to a page that looks like:
  <img width="1728" alt="Screen Shot 2023-01-12 at 4 56 42 PM" src="https://user-images.githubusercontent.com/122579715/212212533-2df0dfdb-d133-4af2-b7ed-70f1aca3cbef.png">
  
  Choose the version that works with your computer and then install it onto your computer. 
  When you're done installing Visual Studio Code, open the application. It should look something like this:
  <img width="1728" alt="Screen Shot 2023-01-12 at 4 19 36 PM" src="https://user-images.githubusercontent.com/122579715/212212657-22d06de7-6012-48c3-ac75-c03405c410d5.png">
  
  
 Step 2: Connecting Remotely:
 
  To log into your ieng6 account, you will first need need to figure out what your account is, which you can do with the following link:
  https://sdacs.ucsd.edu/~icc/index.php
  
  Enter in your UCSD account details and reset your password.
  
  After resetting your password, you will open a terminal on VSCode in order to remotely connect.
  
  You can open the terminal by going to view and then selecting terminal.
  <img width="1728" alt="Screen Shot 2023-01-12 at 5 02 00 PM" src="https://user-images.githubusercontent.com/122579715/212213089-b9ab45b7-7ddd-4ea4-9b63-8df62af66cf9.png">

  **Note: the example of the code that is going to be inputted to your terminal is going to be denoted with a $**
  
  **DO NOT ENTER THE $**
  
  In the terminal, you're going to input the following:
  
  
  **$ ssh cs15lwi23zz@ieng6.ucsd.edu**
  
  
  Before you hit enter, replace the **"zz"** with the letters that are between the **"23"** & **"@"**.
  
  Because this is your first time doing this, it will show this message:
  
  **⤇ ssh cs15lwi23zz@ieng6.ucsd.edu
  The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
  RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
  Are you sure you want to continue connecting (yes/no/[fingerprint])?**
  
  Type in yes, which will prompt you to type in your password.
  
  
  After you type in your password, this will show up in the terminal:
  <img width="901" alt="Screen Shot 2023-01-12 at 4 31 27 PM" src="https://user-images.githubusercontent.com/122579715/212213833-468d8b4b-d2ab-4514-bcc2-980904b8ffb7.png">

  And you'll be all logged in!!
  
  
  Step 3: Trying some commands:
 
   **Here is a list of commands that you can try:**
    
   -cd ~
    
   -cd
   
   -ls -lat
      
   -ls -a
      
   -cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/
      
   -cat /home/linux/ieng6/cs15lwi23/public/hello.txt
      
   You are able to type these into your terminal in VSCode. 
    
   Here is an example:
    
   <img width="744" alt="Screen Shot 2023-01-12 at 4 36 15 PM" src="https://user-images.githubusercontent.com/122579715/212214102-cb9f9834-ac1b-4794-889e-92b40f75c2e0.png">

  When I typed in the cat command, it printed what was inside the hello.txt file.
