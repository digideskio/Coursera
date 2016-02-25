#### Video 03 Notes

##### Week One: History of Cryptography
---
- **History of Crypto**
  - Recommended book: 'The code breakers' by David Kahn (1996)


- **Broken Ciphers**
  - Substitution cipher
    - One letter mapped to another
    - 26! different keys possible if using 26 letters
    - Example: ```E(k, "bcza")```
      - ```k``` represents substitution mapping
    - Broken through letter frequency
      - Calculate frequency of english letters
      - Calculate frequency of pairs of letters
  - Caesar cipher
    - Not really a cipher since it has no key
    - Shift the alphabet by 3
  - Vigenere cipher
    - Key is a word
    - Write the message under the key
    - Replicate the key enough times to cover the message
    - ciphertext for each character = ((key letter + message) % 26)
    - Broken through letter frequency
      - Guess a key size
      - Break ciphertext into blocks of guessed key size
      - Take the first character of each block and calculate frequencies
      - Apply the same principles as the substitution cipher
      - Repeat for each character in the blocks up to guessed key size
  - Rotor machines
    - Early example is the Hebern machine
      - Also broken using statistical attacks
    - Most famous is the enigma machine
  - Digital Ciphers
    - DES
      - Keyspace = 2^56
      - Blocksize = 64 bits
      - Today is considered insecure and should not be used

---

[Back to main](https://github.com/rot0xd/Coursera/blob/master/Cryptography/I/README.md)

