#### Video 04 Notes

##### Week One: Discrete Probability (Crash Course)
---
- **Definitions**
  - ```U``` - Finite set representing universe
    - ex: ```U = {0,1}ⁿ``` represents all strings containing 0 or 1 of length n
  - ```P``` - Probability distribution over ```U``` where ```P:U → [0.1]``` such that ```∑(x∈U): P(x) = 1```
    - Sum of all probabilities of events is 1
    - Examples: Uniform distribution
      - All events in ```P``` have the same weight/probability
      - ```∀x∈U: P(x) = 1/|U|```
    - Point Distribution
      - One event has probability is 1, the rest are 0
      - ```P(x₀) = 1```, ```∀x≠x₀: P(x)=0```
  - Distribution Vector
    - We can write down the entire distribution as a vector since ```U``` is finite
    - ex: ```( P(00), P(01), P(10), P(11) )```
  - Event
    - For a set ```A⊆U: Pr[A] = ∑(x∈A):P(x)∈[0,1]```
    - The set A is called an event
    - Example
      - ```U = {0,1}⁸``` so ```|U| = 256```
      - ```A = {all x in U such that lsb₂(x)=11} ⊆ U```
  - The union bound
    - For events A₁ and A₂ where ```Pr[A₁ ∪ A₂] < Pr[A₁] + Pr[A₂]```
    - If ```Pr[A₁ ∪ A₂] < Pr[A₁] + Pr[A₂]```, then ```A₁ ∩ A₂ = 0```
    - Example
      - ```A₁ = {all x in {0,1}ⁿ such that lsb₂(x)=11}```
      - ```A2 = {all x in {0,1}ⁿ such that msb₂(x)=11}```
      - ```Pr[lsb₂(x)=11 or msb₂(x)=11] = (Pr[A₁ ∪ A₂] ≤ ¼ + ¼) = ½```
  - Random variables
    - Random variable ```X``` is a function ```X:U → V```
    - Generally: ```X``` induces a distribution on V: ```Pr[X=v] := P[X⁻¹(v)]```
    - Example
      - ```X:{0,1}ⁿ  → {0,1}```
      - ```X(y) = lsb(y) ∈ {0,1}```
  - Uniform random variable
    - Let ```U``` be some set, example: ```U = {0,1}ⁿ```
    - We write ```r <-ᴿ- U``` to denote a uniform random variable over ```U```
    - ```∀ a∈U: Pr[r=a] = 1/|U|```
    - Formally, ```r``` is the identity function: ```r(x)=x ∀ x∈U```
  - Randomized algorithms
    - Deterministic algorithm is a function which always gives output ```y``` for input ```x```
    - Random algorithm is a function which always gives random ```y``` for input ```x```
      - Can be thought of as a function that defines a random variable

---

[Back to main](https://github.com/rot0xd/Coursera/blob/master/Cryptography/I/README.md)

