## Encryption vs. Hashing vs. Salting - What's the Difference?

 - Read the article [here](https://www.pingidentity.com/en/resources/blog/post/encryption-vs-hashing-vs-salting.html)
   - Generally speaknig:
     - **Password encryption** is used when the plaintext must be recovered for any reason. Encryption is a reversible method of converting plaintext passwords to ciphertext, and you can return to the original plaintext with a decryption key. Encryption is often used for storing passwords in password managers.
     - **Password hashing** is useful on the server side when server operators don't need to know the plaintext, only that the user knows the plaintext. Hashing is a one-way process that converts a password to ciphertext using hash algorithms. A hashed password cannot be decrypted, but a hacker can try to reverse engineer it.
     - **Password salting** adds random characters before or after a password prior to hashing to obfuscate the actual password. Because of the randomness of the salt, hackers have a very difficult time figuring out actual passwords from hashed salted passwords because their pre-calculated tables of passwords won't work.
 - Another explanation regarding *salt and hash* passwords can be found [here](https://www.okta.com/blog/2019/03/what-are-salted-passwords-and-password-hashing/)