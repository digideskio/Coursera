#### Video 07 Notes

##### Week One: Stream Ciphers and Pseudo Random Generators
---
- **Stream Ciphers**
  - Idea: Replace "random" key by "pseudorandom" key
  - PRG is a function that takes a seed string and outputs a much larger string
    - The function is known as a generator
    - ```G:{0,1}ˢ → {0,1}ⁿ```
      - ```ˢ = len(seed)``` and ```ⁿ = len(output)``` where ```ˢ < ⁿ```
  - Stream ciphers cannot have perfect secrecy

- **Pseudo Random Generators**
  - Must be unpredictable
  - You should not be able to predict any bit in the output
  - Examples of Weak PRG:
    - Linear congruential generator
      - Takes parameters ```a, b, p```
      - ```a,b``` are integers and ```p``` is a prime
      - Very easy to predict
    - glibc random()
      - r[i] ← (r[i-3] + r[i-31]) % 2³²
      - output r[i] >> 1
      - Never use random() for crypto. Very easy to predict


---

[Back to main](https://github.com/rot0xd/Coursera/blob/master/Cryptography/I/README.md)

