# Modular Equivalence and modular arithmetic

## Net Displacement

<img width="169" alt="racetrack" src="https://github.com/user-attachments/assets/da3b75a5-e246-4662-9c5b-8ceaff165a9c" />

Imagine a 5-mile racetrack, with mile markers going 0, 1, 2, 3, 4. The racetrack does a loop, so after 5 miles you'd end up at mile 0. The car's *net displacement* is the total number of forward miles traveled minus the total number of backwards miles. We an characterize the displacement using a numberline, where moving forward corresponds to moving in the positive direction and moving backward corresponds to moving in the negative direction.

### Compute the net displacment:

A. 346 miles in the forward direction, then 432 miles in the backward direction, then 99 miles in the forward direction. **Answer:** 346 - 432 + 99 = 13

B. A forward displacements of 44 miles, followed by 13 additional forward displacements of 53 miles (one after the other). **Answer:** 44 + 13 * 53 = 733

C. Repeat the following sequence 25 times: a forward displacement of 17 miles, followed by a backward displacement of 9 miles, followed by a forward displacement of 22 miles. **Answer:** 25(17 - 9 + 22) = 750

## Position

If we want to represent the *position* of the car on the track as it relates to the net displacement, then we would have to only use 0, 1, 2, 3, 4 on the number line.

<img width="316" alt="01234numberline" src="https://github.com/user-attachments/assets/020a1c1b-3444-480d-a160-d52631627702" />

### Exercises:

D. Compute the positions on the racetrack corresponding to each of the net displacements that you computed.

  A. 13/5 = 3 R (remainder) 3. Position = 3

  B. 733/5 = 146 R 3. Position = 3

  C. 750/5 = 150 R 0. Position = 0

E. How are the answers for the net displacement section related to the exercises in this sections? They are related because no matter the net displacement of the car, dividing it by 5 and taking the remained gives us a number between 0 and 4 (the mile markers), therefore giving us the position.

## Equivlancy

Some displacements correspond to the same position, for example 8, 23, and -17 all correspond to 3 on the racetrack. We say two displacements are *equivalent* if they both correspond to the same position. This may be expressed mathemtically as 8 ≡ 23 (mod 5) (in words, we say '8 is equivalent to 23 mod 5').

How can you tell if they're equivalent?  In our racetrack example we may notice that 8, 23, and -17 all have remainder 3 when divided by 5. So in this example at least, we can see that the position on the racetrack corresponds to the remainder when the displacement is divided by the length of the racetrack (which serves as the modulus). 

But hold on, how do you know if there will always be a remainder? how do you know there's ony one? Why can't some numbers have two remainders or none at all?

## Proposition 1: The Division Algorithm

Given any integer a and any positive integer m, then there exists a unique number r between 0 and m - 1 such that a = q * m + r for some integer q. In this expression, q is called the quotient and r is called the remainder.

### Proof by contradiciton.

Suppose a has two different remainders when dividing by m. let's call these two remainders r and s, where 0 <= r,s <= m-1 and r != s.

