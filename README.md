# Almost Inverse
Implementation of the **Almost Inverse** algorithm, a variant of *Bernstein &amp; Yang* optimized for computing the modular inverse in scalar integers.

# References   
[Paper](https://gcd.cr.yp.to/papers.html#safegcd)

---

**Important Notice:**

 This implementation operates on a finite field of integers 𝔽𝑓, defined by the prime modulo 𝑓. There is no efficiency gain or complexity reduction by using properties of polynomials, as the code was not designed for finite polynomial fields.

 The Almost Inverse algorithm relies on a sufficiently large bit size to function correctly. To ensure proper operation, the following rules must be observed:

- The base `g` must be **less than or equal to the modulus `f`**
- Both the base `g` and the modulus `f` must be **greater than or equal to 32 bits**

---

#### Prerequisites

- g++
- libboost-all-dev

---

## Installation

1. Clone this repository:
    ```bash
    ~/$ git clone https://github.com/lucaselblanc/almostinverse.git
    ```

2. Install the necessary libraries:
    ```bash
    ~/$ sudo apt-get update
    ~/$ sudo apt-get upgrade
    ~/$ sudo apt install g++ libboost-all-dev -y
    ```

3. Compile the project:
    ```bash
    ~/$ cd almostinverse
    ~/almostinverse$ g++ -std=c++14 -O0 almostinverse.cpp -o almostinverse
    ```

4. Run the program:
    ```bash
    ~/almostinverse$ ./almostinverse
    ```