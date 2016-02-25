#### Video 05 Notes

##### Week One: Discrete Probability (Crash Course Continued)
---
- **Recap**
  - ```U: finite set``` - e.g. ```U = {0,1}ⁿ```
  - Probability Distribution ```P``` over ```U``` is a function ```P:U→[0,1] s.t. ∑(x∈U):P(x)=1```
  - ```A⊆U``` is called an event and ```Pr[A] = ∑(x∈A):P(x)∈[0,1]```
  - Random variable ```X``` is a function ```X:U → V```
    - ```X``` takes values in ```V``` and defines a distribution on ```V```


- **Independence**
  - Events ```A``` and ```B``` are independent if ```Pr[A and B] = Pr[A] × Pr[B]```
  - Random variables ```X, Y``` taking values in ```V``` are independent if ```∀(a,b)∈V: Pr[X=a and Y=b] = Pr[X=a] × Pr[Y=b]```
    - Example:
      - ```U = {0,1}² = {00,01,10,11}``` and ```r <-ᴿ- U```
      - Define ```X = lsb(r)``` and ```Y = msb(r)```


- **XOR**
  - XOR of two strings in ```{0,1}ⁿ``` is their bit-wise addition mod 2
  - An important property of XOR:
    - Theorem:
      - Random variable ```Y``` over ```{0,1}ⁿ```
      - Independent uniform variable ```X``` on ```{0,1}ⁿ```
      - ```Z:Y⊕X``` is a uniform variable on ```{0,1}ⁿ```

---

[Back to main](https://github.com/rot0xd/Coursera/blob/master/Cryptography/I/README.md)

