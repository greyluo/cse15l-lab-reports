# Week 4 Lab Report 
    This is a post about how I debugged MarkdownParse java file
    Author: Guidong Luo
## Change 1
1. The screenshot

    ![Image](Images\change1.png)
2. [You can see the test file here](https://github.com/greyluo/markdown-parse/blob/98fd6802a675528b32cf23c100dc6b7339868c67/test-file1.md)


3. Sympstom 
    ![Image](Images\s1.png)
4. Connection
    
    Before, the program would run an error whenever the parenthesises are missing in the test file. 
    
    This is because the last index would be -1 and substring method cannot work in this case.

    To prevent this error, I add a dectector for the parenthesises, so if they are missing, the loop would break. 
## Change 2
1. The screenshot

    ![Image](Images\change2.png)
2. [You can see the test file here](https://github.com/greyluo/markdown-parse/blob/07476fcc87acecd23718b86da172be276fe4bc8e/test-file2.md)


3. Sympstom 
    ![Image](Images\s2.png)
4. Connection
    
    Before, the program would run into a infinite loop, throwing an exception. 

    One possible explanation is that because there is no bracket in the test file, the index would always start with -1. This can run smoothly when there is only one set of link (Not sure why and even so this is not what we want. It is still illegal), but when there are more, the index of the parenthesis can't go on to the next link as the search would start from -1 again. Therefore, the current index would be always smaller than the length, ending in a infinite loop.

    The simple solution to this is to dectect the bracket so that once there is no bracket in the file, the loop would break.

## Change 3
1. The screenshot

    ![Image](Images\change3.png)
2. [You can see the test file here](https://github.com/greyluo/markdown-parse/blob/f7a2b28ceb84950af0cd839e195a2d5ab4e411f8/test-file3.md)


3. Sympstom 
    ![Image](Images\s3.png)
4. Connection
    
   Before, the program seems to run succesfully as no exception being throwed.

   But this is still not we want since they are random texts between the parenthesis and the bracket, which means that this set of link is illegal. 

   This can be resolved by checking the space between the parenthesis and the bracket. Once the space between them is larger than 1, the loop would break.
