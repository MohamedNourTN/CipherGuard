![CipherGuard](https://github.com/MohamedNourTN/CipherGuard/blob/main/icon.ico)
# CipherGuard:

Greetings! Welcome to the GitHub repository CipherGuard! As the name suggests, this application is designed to secure your data through encryption and facilitate its decryption. Additionally, it includes features like Key Derivation Function (KDF), hash, and base64 encoding.

Encryption involves transforming your data into an unreadable format, reversible only with a designated digital key. This program empowers you to perform this crucial function.

To decipher data previously encrypted using a symmetric key encryption algorithm (such as AES or 3DES) within this application, you must possess the "encryption key" used for the initial encryption. This key, comprised of 16, 24, or 32 random characters, serves as the means to both encrypt and decrypt data, earning these algorithms the term "symmetric." Similarly, decrypting asymmetrically encrypted data (utilizing the RSA algorithm) requires a "private key," typically exceeding 1024 characters. For multiple pieces of data to be decryptable with the same private key, they must be encrypted with the corresponding public key, extractable from the private key. Given the involvement of two distinct keys, these algorithms are known as asymmetric.

# Installation:
- $ pip install -r requirements.txt
- $ python main.pyw

# Capabilities:

- Multi-threaded encryption or decryption of plain text or files using AES and 3DES algorithms.
- Capability to create, input, or explore an encryption key, along with the option to save it to a file.
- Encoding and decoding of plain text and files using base64 encoding.
- Calculation of hash values for plain text and files using SHA-1, SHA-256, SHA-512, and MD-5 algorithms.

# Encryption:
![Encrypt](https://github.com/MohamedNourTN/CipherGuard/blob/main/encrypt.png)

![RSA](https://github.com/MohamedNourTN/CipherGuard/blob/main/RSA.png)

The encryption section is specifically designed for the process of encrypting, as implied by its name. Within this feature, the program offers the flexibility to input text or choose a file for encryption. Just below the selection area for the content to be encrypted, users can opt to either generate a new encryption key or utilize a pre-existing one.

In the case of generating a new encryption key, users are presented with two algorithm choices, namely AES or 3DES. Once the algorithm is chosen, users can specify the desired length of the encryption key. Longer keys are more resilient against brute-force attacks, and it's presently deemed impossible to brute-force an AES-256 key. The numeric value following either AES or 3DES indicates the key length in bits, and dividing this number by 8 reveals the character count for the key.

For those opting to enter an existing encryption key, this option is readily available. Users also have the choice to select a key file (*.key or *.txt) saved using the "Save as..." button in the output pane. Upon entering the key, users can further specify the algorithm for encrypting the data below the entry.

To complete the encryption process, users can either press the Enter key on the keyboard or click the "Encrypt" button. The encrypted data is then displayed in the right pane along with the encryption key, which can be used for subsequent decryption. If a file was selected for encryption, the encrypted data is written to the file, unless the "Write encrypted data to the file" checkbox next to the button is unchecked.

# Decryption:
![Decrypt](https://github.com/MohamedNourTN/CipherGuard/blob/main/decrypt.png)

The decryption section, much like its counterpart in the encryption tab, is designed for deciphering data previously encrypted using the encryption tab. Users have the option to input the encrypted data in the large entry field under the "Encrypted text" radio button or choose an encrypted file using the "Browse" button under the "Encrypted file" radio button.

Within the encrypted data selection area, there is an entry for the encryption key that accompanied the encrypted data in the right pane of the encryption tab. Users can either directly input the key or opt to select a key file with extensions *.key or *.txt. Positioned above the entry, users can specify the algorithm employed during the data encryption process.

To complete the decryption process, users, much like in the encryption tab, can click the "Decrypt" button. If the correct encryption key is provided, the decrypted data should be displayed below the button. In cases where a file was selected for decryption, the decrypted data will be written to the file.

# Hash:

This application possesses the capability to perform simple base64 encoding and decoding. Additionally, it is equipped with a Key Derivation Function (KDF) and a hash calculator supporting SHA-1, SHA-256, SHA-512, and MD5 algorithms.
