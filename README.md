# Goldman-Sachs-Engineering-Virtual-Program
Completion of practical task module on Crack leaked password database

## Findings and conclusion of controls implemented by the organization to prevent security breach through successful password cracking

There are several standard cryptographic algorithms that convert plain text to `hashes`, such as SHA-1, SHA-3 (Secure Hash Algorithm), and MD-4, MD-5 (Message Digest) to name a few. However these are subpar techniques to protect data in an organizational level.

All the 19 compromised passwords from the password dump followed `unsalted` MD-5 algorithm, meaning they can be easily ransacked using any password cracker, (i.e., 
crackstation.net , Hashcat.com, dcode.fr/hash-function.com, etc.) 

Terms to get familiar with:

- `hash` - hash is usually a string of characters and the hashes generated by a formula are always the same length, regardless of how much data you feed into it. For example, the MD-5 cryptographic function always produces 32 character-long hashes.

- `salt` - salt is a random string or text that is appended to the data before it is passed onto a hashing function. Salted hashes require more time and computation to be cracked. Strong hashing functions such as 'bcrypt' require salt by default.

There are certain measures that can be taken in order to enhance the data security which is most likely to be compromised if the password policies remain unchanged:

1. Usually the word lists that crackers refer to contain commonly used passcodes that are found in virtually every breach involving consumer 
websites. It is advised to avoid the use of such common passwords like "1234567", "password" (and its other variations like "p@$$w0rd"), 
"pizz@l0ver", etc, because these are extremely weak and can be easily cracked in the first iteration. 

2. The other variable for creating an ease in cracking is usage of memorable words in passwords. Passwords such as "pizzalover" (and its 
variations), or "mom23gr8kidz" contain basic components like "mom", "kid", "pizza", "lover" which become core part of password cracking 
word lists, which with increasing power of hardware and specialized software can be combined together in different permutations for easy 
cracking. Hence, these must be avoided. 

3. Correct usage of complex hashing algorithm like SHA512crypt, bcrypt, scrypt, etc along with salt can defend against brute-force attacks or 
those which require precomputed tables, or rainbow tables. SHA512crypt function included by default in Mac OS X and most Unix-based 
operating systems passes text through 5,000 hashing iterations. Deciphering those hashes require more time and computation.

4. It's also advised to use longer passwords, 8 characters being the starting point. Lengthier passwords are exponentially less likely to be 
accurately guessed, thereby increasing time consumption. 

5. Passwords should not be reused. For better security, passwords should be changed in frequent intervals of time.

6. Users should also avoid using personal information in their passwords which makes them easier to crack.

I, a Computer Science undergraduate, without any prior knowledge of cracking, was able to decipher the password dump of 19 passphrases within 30 minutes. This is not a significant achievement when compared to what extent an experienced cracker could go, hence, a threat to the company's data security which is prone to several vulnerabilities.

After cracking the passwords, I found the following things about organisation’s password policy: 

• Minimum length for password is set to 6.

• There is no specific requirement for the password creation. Users are able to use any combination of word and letters to create a password, 
and even including personal details in most cases.


I think the current password policy, because of it being prone to numerous susceptibilities, must be revised. My recommendations include:

1. Increasing password length to a minimum of 9 characters, while enforcing the use of 13 characters to create strong passwords through 
password strength checker. 

2. Avoiding common words, previously used passphrases, personal details while creating passwords. 

3. Using varieties of special characters, capital and small letters, and numbers during password creation. 

4. Promoting safe storage and change of passwords in regular intervals to avoid any data leak/compromise. 

5. Training users to follow these policies in order to keep their passwords safe. 

This is basically what the content of my report is. However, below attached is a link to my report for your reference

[Report](https://drive.google.com/file/d/13HrF3VXI7Oyxo3ioaY5Zd2jB7XRlftZW/view?usp=sharing)

Also, here is a chart that I made, containing username, corresponding hash, hashing function followed and the decrypted password.

![IMG_20220323_204625](https://user-images.githubusercontent.com/80174214/159733321-627ce644-21b5-424b-99b3-377623308f16.jpg)

Here is the link to the Password Dump:
[Password Dump](https://cdn.theforage.com/vinternships/companyassets/MBA4MnZTNFEoJZGnk/passwd_dump.txt)

## Tools

• https://hashcat.net/hashcat/

• https://dcode.fr/hash-function.com/

• https://crackstation.net/

• https://en.wikipedia.org/wiki/Password_cracking#Software


## Resources

• https://arstechnica.com/information-technology/2013/05/how-crackers-make-minced-meat-out-of-your-passwords/

• https://en.wikipedia.org/wiki/Salt_(cryptography)

• https://en.wikipedia.org/wiki/Cryptographic_hash_function
  
• https://howsecureismypassword.net/
