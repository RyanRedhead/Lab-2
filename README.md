Basic Cryptography
==================
#Purpose

To decrpyt bytes with a key using subroutines.

#Flow Chart

![Alt Text](https://github.com/RyanRedhead/Lab-2/blob/master/photo.JPG?raw=true)

#Hardware Schematic

Simply the board connected to the computer, same as Lab 1.

#Debugging

Using different register modes to select the right data and put it in the right place took some time to figure out.

#Testing Methedology/Results

 The length of the message was found by subtracting the encryption address with the key address. The length was then decremented after each byte to test if ended/zero. An encrypted byte was put into r10 where it was XOR'd with the key, the decrpyted data was then put in the appropriate memory location. Subroutines to decrpyt a byte and then a subroutine within that one was used to decrpty a character. To view the characters or message you had to look at the character option in memory. The required functionality gave the following: 

#Observations/Conclusions

The first A functionality could have been achieved by making a loop and like 3rd grade math, adding a number to another number that many times. Ex. 4 x 3 = 4 + 4 + 4. I tried to go for the harder A functionality using shift-adds to multiply but I'm not sure why my program doesn't work.

#Documentation: 
I added more to my flow chart after Dr York checked it and commented on expanding the operations. Also, Dr York explained how to shift and add to create a multiplier that would achieve A functionality. 

