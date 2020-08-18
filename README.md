**# The Odin Project - Ruby Programming**

**### Project: Caesar Cipher**

###Introduction:
In cryptography, a Caesar cipher, also known as Caesar’s cipher, the shift cipher, Caesar’s code or Caesar shift, is one of the simplest and most widely known encryption techniques. It is a type of substitution cipher in which each letter in the plaintext is replaced by a letter some fixed number of positions down the alphabet. For example, with a left shift of 3, D would be replaced by A, E would become B, and so on. The method is named after Julius Caesar, who used it in his private correspondence.

This project is part of The Odin Project’s Ruby Programming [curriculum](https://www.theodinproject.com/courses/ruby-programming/lessons/caesar-cipher?ref=lnav).

**### Solution:**

    • Function is called with two arguments – a string, and the desired ‘offset’
    • The string is iterated over to check whether each character exists in an array of alphabet letters
    • If the character is found, the offset value is added to the character’s index
    • To ensure that the new index is within the index range of the array, the modulus is calculated using the modulo operator
      with the length of the array. e.g. 28 % 26 = 2. This ensures that the index always ‘rotates’ around the 26 possible indexes.
    • The character at the new index is added to an array of results
    • If the character wasn’t found in the array, the original character is added to the results array
    • The results array is returned
