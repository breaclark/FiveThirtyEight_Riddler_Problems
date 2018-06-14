# FiveThirtyEight Riddler Problem

### By Brea Clark

### The Premise: http://fivethirtyeight.com/features/can-you-best-the-mysterious-man-in-the-trench-coat/

Basically, if you guess the correct number between 1 and 1000, you get that amount of money.

Let's start with the basic approach. Say you start with 500, and you're going to do a binary search, where you guess 500, he says higher or lower, then you pick the number in the middle there (either 250 or 750), etc.
The problem there is that once you get to your 4th guess (and onward), there is not an exact middle number to guess. So maybe you just round up each time and keep going, and on your 9th guess you have at best a 33% chance of getting the money, which is not bad.

But we could make it better by maximizing these guesses where you would otherwise just round up a number. If you were to originally pick a number a little higher up, then you would eliminate those times where you just round up, getting you a more accurate 9th guess. Let's start with the number 512. 512 = 2^9. This is significant because that means that every step of the way, we will have a middle number to guess, and will not "waste" a guess on a non-middle number.

## Setup/Installation Requirements

* Clone Repository
* Ensure Jupyter notebooks can run
* Open Number Guesser Problem.ipynb	 in Browser

## Known Bugs

No Known Bugs

## Support and contact details

Contact me at breatortilla@gmail.com

## Technologies Used

* Python

### License

Copyright (c) 2018 **Brea Clark**
