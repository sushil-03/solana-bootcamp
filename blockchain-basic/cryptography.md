# Cryptography

Cryptography is the practice of securing information and communication through the use of codes, ciphers, and cryptographic algorithms.

## Hash Functions

Hash functions are functions that take an input and return a fixed-size string of bytes. The output string is called the **hash**.

## Encryption

- **Encryption**: The process of encoding a message or information so that only authorized parties can read it.
- **Decryption**: The process of decoding an encrypted message so that authorized parties can read it.

## Hashing

- **Hashing**: The process of encoding a message or information in such a way that it cannot be read or altered without the key.
- **Irreversibility**: Hashing is irreversible, meaning the original input cannot be retrieved from the hash.

## Public Key Cryptography

- **Definition**: A method of encrypting data so that only authorized parties can read it.
- **Key Pair**: Utilizes a pair of keys: a **public key** and a **private key**.
  - The **public key** is used to encrypt the data for sharing.
  - The **private key** is used to decrypt the data, ensuring only the authorized party can read it.

## Digital Signature

- **Definition**: A mathematical scheme for verifying the authenticity of digital messages or documents.
- **Uses**: Verifies the authenticity, integrity, and non-repudiation of a message or document.

## Key Pair

- **Definition**: A pair of keys consisting of a public key and a private key.
- **Functionality**:

  - The **public key** encrypts the data for sharing. It can be shared with anyone.
  - The **private key** decrypts the data, allowing only the authorized party to read it. It should never be shared.

- **Workflow**:
  - Sender encrypts the data using the receiver's public key.
  - Receiver decrypts the data using their private key.
  - Receiver sends the data back to the sender encrypted with their private key.
  - Sender decrypts the data using the receiver's public key.

**DOUBT**: How will the data only get decrypted by the receiver's private key when it is encrypted with receiver public key?

> The encryption process uses the receiver's public key, which is mathematically linked to their private key. Only the corresponding private key can decrypt the data that was encrypted with the public key. This ensures that even if the encrypted data is intercepted, it cannot be decrypted without access to the private key.
