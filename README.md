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
* Day 11: **TODO**
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
* [Day 17](Day%2017.ipynb): 2020-02-04
  * Maze navigation with DFS with a MD5 to determine wall configuration at each step, depending on previous moves. Fun!
* [Day 18](Day%2018.ipynb): 2020-01-31
  * Iterative building similar to a 1-D Conway's Game of Life
* [Day 19](Day%2019.ipynb):
  * Part 1: 2020-02-01. Coded a poor-man linked list with delete, but it's not very inefficient to solve the full example. Found a clever algorithm to solve it just by reducing list of playing elves in cumulative way. 
  * Part 2: 2020-02-03. Coded a list-based approach as for Part 1, then looked for patterns in solutions with small values. Found patterns, coded fast solution exploiting them! 
  * After the fact, found out this is variation on a very very old problem known as [Josephus problem](https://en.wikipedia.org/wiki/Josephus_problem). See for instance this [Numberphile video](https://www.youtube.com/watch?v=uCsD3ZGzMgE).
* [Day 20](Day%2020.ipynb): 2020-02-02
  * Overlapping and contiguous interval merging using a simple stack (implemented with a `list`)
* [Day 21](Day%2021.ipynb): 2020-02-02
  * More list manipulation, then brute force using `itertools` `permutations`
* [Day 22](Day%2021.ipynb): 
  * Part 1: 2020-02-03. Simple tuple counting
  * Part 2: **TODO**
* [Day 23](Day%2021.ipynb): 2020-02-03
  * An extension of the assembly code of Day 12. Part 1 one easy, part 2 took > 1h to brute force, but understanding what the code was doing could lead to instantaneous solution. One could also have tries to implement an optimization of assembly multiplication implemented as sum, but this was too far away from my skill-set...
* [Day 24](Day%2024.ipynb): 2020-02-04
  * Maze solving with special location to visit at least once. Similar to AOC 2019 Day 19 with keys to collect to open doors. 
  * Solution with DFS and steps on paths represented by 2D spatial coordinates plus list of special locations visited. 
  * Slight modification for Part 2 to go considering going back to initial position as condition.
* [Day 25](Day%2024.ipynb): 2020-02-04
  * A final `assembunny` puzzle, now with an output instruction.
