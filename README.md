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
![Alt Text](https://github.com/RyanRedhead/Lab-2/blob/master/decrypt.PNG?raw=true)

#Observations/Conclusions

B functionality could have been aciheved by looking seperating the known key into 3 seperate bytes and creating a loop to decrypt a byte, move to the next key byte, decrpyt, and so on. Resetting the key loop when it uses all key bytes once.

A functionality I did not even look at.

#Documentation: 
Dr. York corrected my flow chart; the decrypt character subroutine is not in the top level because it is referenced in the decrypt message sub routine. 

