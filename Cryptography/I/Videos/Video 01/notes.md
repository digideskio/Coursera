#### Video 01 Notes

##### Week One: Course Overview
---
- **Course Objectives**
  - Learn how crypto primitives work
  - Learn how to use them correctly and reason about security


- **Course Recommendations**
  - Take notes
  - Pause frequently
  - Answer questions


- **Crypto is everywhere**
  - Secure communication
    - HTTPS, 802.11i WPA2, GSM, Bluetooth
  - File encryption
    - EFS, TrueCrypt
  - Content Protection
    - DVD (CSS), Blu-ray (AACS)
  - User Authentication
  - Many more applications....


- **Secure Communication**
  - Data travels across the network
  - Two main goals
    - No eavesdropping by attacker
    - No tampering by attacker


- **SSL/TLS**
  - SSL: Secure Sockets Layer
  - Two main parts
    - Handshake Protocol
      - Establish shared secret key using public-key cryptography
    - Record Layer
      - Transmit data using shared secret key
      - Ensure confidentiality and integrity


- **File Encryption**
  - Analagous to secure communication
    - File encryption is communication with future self
  - Two main goals
    - File cannot be viewed by attacker
    - No tampering by attacker


- **Symmetric Encryption Building Blocks**
  - Variables
    - ```E``` - Encryption Algorithm
    - ```D``` - Decryption Algorithm
    - ```k``` - Secret Key
    - ```m``` - Plaintext Message
    - ```c``` - Ciphertext
  - Definitions
    - E(k,m) = c
    - D(k,c) = m
  - Encryption algorithm is publicly known
  - Never use a proprietary cipher
  - Only thing kept secret is ```k```


- **Key Usage**
  - Single-Use Key (One-Time Key)
    - Key is only used to encypt a single message
    - Used in encrypted email. (New key generated every e-mail)
  - Multi-Use Key (Many-Time Key)
    - Key is used to encypt multiple messages
    - Used to encrypt files. (Same key encrypts many files)
    - Need more machinery than for one-time key


- **Things To Remember**
  - Cryptography
    - A tremendous tool
    - The basis for many security mechanisms
    - NOT the solution to all security problems
      - Will not help with software bugs
      - Will not stop social engineering attacks
    - NOT reliable unless implemented/used properly
    - NOT something you should invent yourself
      - Many examples of broken designs

---

[Back to main](https://github.com/rot0xd/Coursera/blob/master/Cryptography/I/README.md)

