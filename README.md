# Almost Inverse
Implementation of the **Almost Inverse** algorithm, a variant of *Bernstein &amp; Yang* to calculate the modular inverse of arbitrary integers.

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
