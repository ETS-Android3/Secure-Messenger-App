# Secure-Messenger-App

 An Android application to have secure communication between the sender and recipient, using cryptography algorithm(AES) for encryption and decryption.

The AES algorithm (also known as the Rijndael algorithm) is a symmetrical block cipher algorithm that takes plain text in blocks of 128 bits and converts them to ciphertext using keys of 128, 192, and 256 bits. Since the AES algorithm is considered secure, it is in the worldwide standard.


## High-level description of the algorithm
1.**KeyExpansion** – round keys are derived from the cipher key using the AES key schedule. AES requires a separate 128-bit round key block for each round plus one more.


2.**Initial round key addition**:
AddRoundKey – each byte of the state is combined with a byte of the round key using bitwise xor.


3.**9, 11 or 13 rounds**:
SubBytes – a non-linear substitution step where each byte is replaced with another according to a lookup table.
ShiftRows – a transposition step where the last three rows of the state are shifted cyclically a certain number of steps.
MixColumns – a linear mixing operation which operates on the columns of the state, combining the four bytes in each column.
AddRoundKey

4.**Final round (making 10, 12 or 14 rounds in total)**:
SubBytes
ShiftRows
AddRoundKey
 
