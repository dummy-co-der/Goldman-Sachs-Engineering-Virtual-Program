# Goldman-Sachs-Engineering-Virtual-Program
Completion of practical task module on Crack leaked password database

## Review of the Password Leak and Policy Changes.

Secure Hash Algorithm (SHA) and Message Digest (MD5) are the standard cryptographic hash functions to provide data security for authentication.  All the 19 compromised passwords followed unsalted MD-5 algorithm, meaning they can be easily ransacked using any password cracker.

Considering the results of the cracking of leaked passwords, it can be concluded that your password policy is prone to several vulnerabilities.  This email concludes all the findings and suggestions to improve your password policy.

### 1. In the Event of a future password database leak following controls should be implemented to make the cracking much harder:
•	Improve the current password policy of the organisation. <br>
•	Employees must be aware of the password ethics. <br>
•	Using of secure hashing algorithm like SHA or Symmetric Cryptographic Algorithm is recommended. <br><br>

### 2.	Observations made regarding organization’s policy:
•	Minimum length of password is set to 6. <br>
•	There is no specific requirement for the password creation.  Employees can use any combination of word and letters to create a password. <br>
•	No checks were made to ensure capital and special characters in password. <br><br>

### 3. Changes recommended in password policy:
•	Don’t let the employees include their username, actual name, date of birth and other personal information while creating a password. <br>
•	Increasing password length to a minimum of 9 characters, while enforcing the use of 13 characters to create strong passwords through password strength checker. <br>
•	There should be at least 1 capital letter and 1 special character in password. <br>
•	Avoid using common password elements like username, sequence of numbers etc. <br>
•	Promoting safe storage and change of passwords in regular intervals to avoid any data leak/compromise. <br>

This is basically what the content of my report is. However, below attached is a link to my report for your reference

[Report](https://drive.google.com/file/d/10OfwHO8Xf_z9FTYZFkuunzb3H1510jYS/view?usp=sharing)

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
