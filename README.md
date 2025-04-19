### ECDSA

## Quadratic Residue 
Imagine a clock with `n` total ticks. Now, the quadratic residue is the number by which the square of a number `q` overshoots. 

Taking an example from Grok: 
- Take modulus 7 (the clock has numbers 0, 1, 2, 3, 4, 5, 6).
- Square some numbers:
  - \( 1^2 = 1 \)
  - \( 2^2 = 4 \)
  - \( 3^2 = 9 \), but on the clock, \( 9 - 7 = 2 \), so it’s 2.
  - \( 4^2 = 16 \), and \( 16 - 14 = 2 \), so also 2.
  - \( 5^2 = 25 \), and \( 25 - 21 = 4 \), so 4.
  - \( 6^2 = 36 \), and \( 36 - 35 = 1 \), so 1.
- The numbers you get are 0, 1, 2, 4. These are the quadratic residues for mod 7.

## Tonelli-Shanks Algorithm
It is a method to find a number `x` such that $x^2 = a(\mod p)$ where `a` is a quadratic residue modulo a prime number `p`. 