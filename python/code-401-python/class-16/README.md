[MainPage](../../../README.md)
# Encrypting
Encrypting a message
Imagine Caesar wants to send this message:
SECRET MEETING AT THE PALACE
Here's what that might look like encrypted:
YKIXKZ SKKZOTM GZ ZNK VGRGIK
That looks an awfully lot like gobbledygook at first, but this encrypted message is actually very related to the original text.
The Caesar Cipher is a simple substitution cipher which replaces each original letter with a different letter in the alphabet by shifting the alphabet by a certain amount.
# Frequency analysis
Human languages tend to use some letters more than others. For example, "E" is the most popular letter in the English language. We can analyze the frequency of the characters in the message and identify the most likely "E" and narrow down the possible shift amounts based on that.
# Known plaintext
Another term for the original unencrypted message is plaintext. If the enemy already knew some part of the plaintext, it will be easier for them to crack the rest of the encrypted version.
For example, messages tend to start with similar beginnings. In WWII, encrypted German messages always started with a weather forecast, which ultimately made them easier for British mathematician Alan Turing to crack.
Do you think Julius started this message in a common way?
Encryption, decryption, and cracking
Thanks to this exploration of the Caesar Cipher, we now understand the three key aspects of data encryption:
Encryption: scrambling the data according to a secret key (in this case, the alphabet shift).
Decryption: recovering the original data from scrambled data by using the secret key.
Code cracking: uncovering the original data without knowing the secret, by using a variety of clever techniques.
Whenever we consider a possible encryption technique, we need to think about all those aspects: how easy is it to encrypt? how easy is it to decrypt? And most importantly, how easy is it for a nefarious individual to crack the code?
We can no longer use the Caesar Cipher to secure our data, as it is far too easy to crack, but understanding the Cipher prepares us for understanding modern encryption techniques.