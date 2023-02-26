# Done Quick Lab

## Intro to the Lab:

  In this lab, we learned how to use nano to make a change in a file and have it be pushed into a github repository. This was done by
  doing a series of tasks as quickly as possible for the reward of a pass on the next Skill Demo. 
  
  ## Here are the Steps
  1. Setup Delete any existing forks of the repository you have on your account
  2. Setup Fork the repository
  3. The real deal Start the timer!
  4. Log into ieng6
  5. Clone your fork of the repository from your Github account
  6. Run the tests, demonstrating that they fail
  7. Edit the code file to fix the failing test
  8. Run the tests, demonstrating that they now succeed
  9. Commit and push the resulting change to your Github account (you can pick any commit message!)

  I will be going through steps 4-9 and I will explain how they were done.
  
  ## Step 4: Log into ieng6
  First, I logged into my ssh account. I did this by opening the terminal in Visual Studio Code and typing the following:
  
    bdikbas@Buraks-MacBook-Pro PA6 % ssh cs15lwi23avh@ieng6.ucsd.edu 
    Keys Pressed: <enter>
 
  and then I hit the enter key to follow through with the login so that I could continue with the steps.
  
  <img width="1237" alt="Screen Shot 2023-02-25 at 4 55 06 PM" src="https://user-images.githubusercontent.com/122579715/221386576-a4e83192-423c-40b2-9f10-76b2a43f4b50.png">

  ## Step 5: Cloning the fork of the repository from my Github account
  After I forked the repository during the setup, I copied the ssh key with <ctrl+c> and then utilized the git clone command to get it into my account.
  It is important to use the ssh link instead of the actual https:// link in order to add and push changes onto the github page. After copying the ssh link, I used <ctrl+v> to paste it into the command line in order to clone the repository into my account. The enter key was used
  to finish the task. I also used the ls command before and after to show the lab7 repository not being in the
  
    [cs15lwi23avh@ieng6-203]:~:505$ git clone git@github.com:bdikbas/lab7.git 
    Keys pressed: <ctrl+v> <enter>
  
  ![Screen Shot 2023-02-25 at 5 01 03 PM (2)](https://user-images.githubusercontent.com/122579715/221386807-85d457d2-b242-495c-96b9-2ad742988db8.png)

  <img width="929" alt="Screen Shot 2023-02-25 at 5 04 14 PM" src="https://user-images.githubusercontent.com/122579715/221386820-aff1ebee-f729-4b35-982f-a59c5a61ebde.png">

  ## Step 6: Running the tests
  In order to run the JUnit tests, I changed my directory into the newly cloned lab7 directory. I did this typing in cd and then l, followed by a <tab>
  to autocomplete the line, and then I hit enter to complete the task. 
  
    [cs15lwi23avh@ieng6-203]:~:507$ cd lab7/
    Keys Pressed: <tab> <enter>
  
  After that, I went to Week 3 to copy <ctrl+c> the command to compile JUnit and the other two finals inside lab7, ListExamples.java and ListExamplesTests.java.
  
     [cs15lwi23avh@ieng6-203]:lab7:511$ javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java
     [cs15lwi23avh@ieng6-203]:lab7:512$ java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests 
     Keys Pressed: <ctrl+v>, <enter>, <ctrl+v>, <tab>, <backspace>, <enter>
  
  <ctrl+v> was used to paste the two commands into the command line. For the java command, I used tab after typing L and T to autocomplete the ListExamplesTests.
  The backspace was used to get rid of the extra period at the end of ListExamplestests.
  
  <img width="1285" alt="Screen Shot 2023-02-25 at 5 14 50 PM" src="https://user-images.githubusercontent.com/122579715/221387061-bda14387-6331-4856-9067-4a7ce570203c.png">

   After the test ran, we can see that there are two tests with one of them having an error.
    
## Step 7: Fixing the code
      
