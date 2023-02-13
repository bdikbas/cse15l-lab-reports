## Part 1

**Lab Intro**
In this lab, we learned how to use and understand how to use symptoms to find and correct bugs with the help of a Visual Code Studio extension called JUnit. JUnit is used to test certain inputs and makes sure that the expected output matches the actual ouput.

<img width="398" alt="Screen Shot 2023-01-29 at 5 42 41 PM" src="https://user-images.githubusercontent.com/122579715/215370502-29761dc9-5735-4c76-b750-f80652b4dc8d.png">

**Which methods in your code are called?**

In this screenshot, the handleRequest method is called in order to help print the word "Hello" on the page with the help of the Server.java we used in the second lab.

**What are the relevant arguments to those methods, and the values of any relevant fields of the class?**

The relevant argument is a URI object of the url. The relevant fields is the StringBuilder, which keeps track of each message that is added to the page. Every time the add-message is used, a word will appear below the last word inputted. Stringbuilder message is used to keep track of the words inputted while Stringuilder keyword is used to append the next word to message. The String[] parameters is used to extract the keyword that will be appended to the message that is going to be printed onto the screen.

**How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.**

The relevant values get changed by the new word being appended to the end of the word in addition to a "\n" so that the website can print the next word below the previously inputted word.


<img width="618" alt="Screen Shot 2023-01-29 at 7 30 47 PM" src="https://user-images.githubusercontent.com/122579715/215381692-3b529b58-770a-4e2a-b4d1-7a4b47eed7b6.png">

**Which methods in your code are called?**

In this screenshot, the handleRequest method is called in order to help print the words "How Are You" on the page with the help of the Server.java we used in the second lab.

**What are the relevant arguments to those methods, and the values of any relevant fields of the class?**

The relevant argument is a URI object of the url. The relevant fields is the StringBuilder, which keeps track of each message that is added to the page. Every time the add-message is used, a word will appear below the last word inputted. Stringbuilder message is used to keep track of the words inputted while Stringuilder keyword is used to append the next word to message. The String[] parameters is used to extract the keyword that will be appended to the message that is going to be printed onto the screen.

**How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.**

The relevant values get changed by the new word being appended to the end of the word in addition to a "\n" so that the website can print the next word below the previously inputted word.


**Here is the code for the StringServer**
<img width="1373" alt="Screen Shot 2023-01-29 at 7 33 17 PM" src="https://user-images.githubusercontent.com/122579715/215381945-869cf878-16ba-40aa-b1a3-0e16de44b60e.png">

## Part 2

  In the Array Examples file, the testReversed() function had a bug that caused the array to not be printed backwards. The symptom that shows up in the terminal is the original array that is inputted being instead of the inputted array reversed. A failed input would be the following:

    @Test
     public void testReversed() {
      int[] input1 = { 1, 2, 3, 4, 5 };
      assertArrayEquals(new int[]{5, 4, 3, 2, 1 }, ArrayExamples.reversed(input1));
    }

    static int[] reversed(int[] arr) {
      int[] newArray = new int[arr.length];
      for(int i = 0; i < arr.length; i += 1) {
        arr[i] = newArray[arr.length - i - 1];
      }
      return arr;
    } 
    
   ![Screen Shot 2023-01-29 at 3 58 24 PM](https://user-images.githubusercontent.com/122579715/215363514-608264eb-3c6f-495b-9d28-1b09111bab3e.png)
    
  This would lead to the original array to become all 0's due to the newArray being copied into the orignial array. However, if the input Array was all 0's, then the test would be successful. The symptom woulnd't show up in the terminal.
  
      @Test
      public void testReversed() {
        int[] input1 = {0, 0, 0};
        assertArrayEquals(new int[]{0, 0, 0}, ArrayExamples.reversed(input1));
      }
  
      static int[] reversed(int[] arr) {
          int[] newArray = new int[arr.length];
          for(int i = 0; i < arr.length; i += 1) {
              arr[i] = newArray[arr.length - i - 1];
          }
          return arr;
    } 
    
   ![Screen Shot 2023-01-29 at 3 57 46 PM](https://user-images.githubusercontent.com/122579715/215363524-6707336e-29de-4918-ba27-d98d28d0bf92.png)

   The bug is the fact that the contents of the input array aren't being copied into the newArray. In addition to that, the newArray isn't even being returned.
   
   **Before**
   
          static int[] reversed(int[] arr) {
              int[] newArray = new int[arr.length];
              for(int i = 0; i < arr.length; i += 1) {
                arr[i] = newArray[arr.length - i - 1];
              }
              return arr;
          } 
   **After**
   
            static int[] reversed(int[] arr) {
                int[] newArray = new int[arr.length];
                for(int i = 0; i < arr.length; i += 1) {
                    newArray[i] = arr[arr.length - i - 1];
                }
                return newArray;
              } 
              
   This fixes the issue because now, the input array is able to copied into the newArray in reverse order, which is what we want the function to be able to do. The symptom that was showing up before hand in the terminal doesn't anymore due to the correct array being returned.
   
## Part 3
   
   Something that I learned from week 2 was how to create my own Server and be able to increment a number on the page with the help of the URI Class & String Class.
   I didn't know how the split command was used in the String class for it to split different parts of the url into different parts of the array. But after doing this lab,
   I have a deeper understanding toward how to use both of these classes together in order to succeed in the task at hand during the lab.
  
