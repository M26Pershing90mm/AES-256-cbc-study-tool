AES 256 cbc study tool
A simple pure Python AES-256-CBC encryption and decryption tool made for study and learning purposes.
This project implements AES-256-CBC directly in Python without using external cryptography libraries.
Features
AES-256-CBC encryption
AES-256-CBC decryption
Random 256-bit key generation
Random 128-bit IV generation
UTF-8 text support
Hexadecimal ciphertext output
No external Python packages required
Requirements
Python 3
No additional packages are required.
Usage
Run the script:
python AES Tool.py
The program will display:
1. Encrypt
2. Decrypt
3. Exit
Encrypt
Select:1
Enter the text you want to encrypt:
Text:Hello World
The program automatically generates a random AES-256 key and IV.
Example output:
Key:64-character hexadecimal key
IV:32-character hexadecimal IV
Cipher:encrypted hexadecimal data
Save the Key,IV and Cipher values if you want to decrypt the text later.
Decrypt
Select:2
Enter the values generated during encryption:
Key:(your key)
IV:(your iv)
Cipher:(your ciphertext)
If the values are correct, the original text will be displayed:
Text:Hello World
Exit
Select:3
to exit normally.
Entering 0 at an input prompt will exit the program immediately.
Technical Information
Algorithm: AES-256
Mode:CBC
Key size:256 bits
Block size:128 bits
IV size:128 bits
Padding:PKCS#7
Text encoding:UTF-8
Ciphertext format:Hexadecimal
Random key and IV generation:Python secrets module
File Information
File Name:AES Tool.py
Size:1 MB
MD5:3d5e2f2ccc6a6c5041f5b487fefc4f54
SHA-1:04f617d67c840a66fa0a502ed523157f9b6081b3
SHA-256:8f8334a57f884239164dc4bcae7a8dcb3d19a0f99842c2754ccf0830debd42e6
Note
This project was created for educational and study purposes.
AES-CBC provides encryption but does not provide built-in authentication or integrity protection. For security-sensitive real-world applications, an authenticated encryption mode such as AES-GCM is generally more appropriate.