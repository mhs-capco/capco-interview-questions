# General Interview questions

# Language Agnostic Coding questions
## anagrams
### Problem
given a paragraph, provide a list of words that are anagrams of eachother. Anagrams are collections of strings that have the same character inventories.

Single word example: Elvis <=> Lives

Sample input: `What can we glean from an angel?`

expected output(or something similar): `[[glean, angel]]` (no ordering is specified)
### Expectations
The essence of this is task is detecting permutations, or in other words, creating a way to look at a string's contents independent of order.  

Three flavors of solution include:
- reordering the strings
- inventorying the characters in in string and comparing the inventories
- creating a "bad" hash function that doesn't change when the input strings are permuted

We expect top candidates to quickly decide to reorder the inputs using a library sort. Some candidates may need hints as to permutations, and ways to detect them.

All candidates are expected to select an appropriate container collect anagrams and be able to iterate over it to provide an output.

## list addition
### Problem
given two lists of digits representing multidigit numbers, in order of decreasing significance, implement decimal integer addition.
#### examples
1. [1,2,3] + [3,2,1] => [4,4,4]
### expectatons
#### cases
the development of test cases that discover edge cases.
eg:
1. carrying over
1. lists of unequal length
#### libraries
1. familiarity with modulo operator
1. ways ways of iterating over two lists
   - for each in join
   - for i in lenth shorter
#### algorithms
- How does the candidate iterate backwards?
- do they use three-value addition?
- how do they pad to equal lengths? If they do.


