# Advent Of Code 2016

My solutions to the [2015 Advent Of Code](https://adventofcode.com/2016) puzzles.

I did not participate to the challenge in 2016 (my first was in 2019) but I decided it would have been fun (and good practice) to try to solve them in my spare time.

## ChangeLog and Notes

* [Day 1](Day%2001.ipynb): 2020-01-28
  * 2-D grid navigation using complex numbers to store coordinate and (change of) directions
  * Manhattan distance
* [Day 2](Day%2002.ipynb): 2020-01-28
  * Again 2-D movements, again using complex numbers for coordinates and boundary checks
* [Day 3](Day%2003.ipynb): 2020-01-28
  * Quick use of RegExp to simplify parsing of input
* [Day 4](Day%2004.ipynb): 2020-01-28
  * `Counter` to count character frequency in string
  * Caesar shift cipher implemented with `str.maketrans()`
  * Iterative manual solution of second part!
* [Day 5](Day%2005.ipynb): 2020-01-29
  * MD5 hashing
* [Day 6](Day%2006.ipynb): 2020-01-29
  * `Counter` plus some list manipulation
* [Day 7](Day%2007.ipynb): 2020-01-29
  * String slicing, manipulation and comparing
* [Day 8](Day%2008.ipynb): 2020-01-29
  * `numpy` array slicing and broadcasting
  * `matplotlib` for visualisation
* [Day 9](Day%2009.ipynb): 2020-01-30
  * String manipulation for Part 1
  * Using iteratively solution for Part 1 cannot really work for Part 2 (too large string) even if it's fine for example. 
  * Part 2 solution uses "compressed" information: assuming each decompressed repeating item can be decompressed by itself (e.g. no overlapping on chain of repeating items: it makes sense if this really was a compression algorithm), I save the single repeating item and the number of times it should repeat in the final string. Details in notebook.
* [Day 10](Day%2010.ipynb): 2020-01-30
   * Iterative execution of possible instructions given system state, saving and avoiding repeating already-executed instructions, until exhaustion of all instructions.
* Day 11: 
* [Day 12](Day%2012.ipynb): 2020-01-30
   * Pseudo-assembly code (learned my lessons with AOC 2019 Intcode!)
* [Day 13](Day%2013.ipynb): 2020-01-31
  * Maze solving using DFS (code from AOC 2019!)
* [Day 14](Day%2014.ipynb): 2020-01-31
  * MD5 + RegExp string searching
  * Caching/memoizing already implemented to speed up Part 1 made Part 2 accessible!
* [Day 15](Day%2015.ipynb): 2020-01-31
  * Effectively a prime number reminder problem, it could probably be solved with Chinese Reminder Theorem (see AOC 2020)
  * Size was nevertheless small enough even for Part 2, and direct search simply worked!
* [Day 16](Day%2016.ipynb): 2020-01-31
  * String manipulation, slicing, comparing.
* Day 17: 
* [Day 18](Day%2018.ipynb): 2020-01-31
  * Iterative building similar to a 1-D Conway's Game of Life
* Day 19: 
* Day 20:
* Day 21:
* Day 22: 
* Day 23:
* Day 24:
* Day 25:
