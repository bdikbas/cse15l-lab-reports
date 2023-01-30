## Part 1







## Part 2
**The Bug**:

The Bug from Lab 3:

  In the Array Examples file, the testReversed() function had a bug that caused the array to not be printed backwards. A failed input would be the following:

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
    
  This would lead to the original array to become all 0's due to the newArray being copied into the orignial array.
  
  However, if the input Array was all 0's, then the test would be successful.
 
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

   The bug is the fact that the contents of the input array aren't being copied into the newArray. In addition to that, the newArray isn't even
   
   being returned.
   
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

  
   This fixes the issue because now, the input array is able to copied into the newArray in reverse order, which is what we want the function to be able to do.
   
## Part 3
   
   Something that I learned from week 2 was how to create my own Server and be able to increment a number on the page with the help of the URI Class & String Class.
   I didn't know how the split command was used in the String class for it to split different parts of the url into different parts of the array. But after doing this lab,
   I have a deeper understanding toward how to use both of these classes together in order to succeed in the task at hand during the lab.
  
