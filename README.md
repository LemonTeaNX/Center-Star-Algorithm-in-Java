# Center-Star-Algorithm-in-Java
Center star algorithm for minimizing the sum-of-pairs objective with minimum edit distance weights (i.e., cost of 1 for indels and mismatches, and cost of 0 for matches, including matches between 2 spaces). The algorithm has two main steps. Given n strings s1,.., sn, in the first step we find an index c such that edit_dist(si, sc) is minimized. In the second step, a multiple alignment is constructed by successively aligning each string si to sc, for i not equal to c.
Center star algorithm is implemented using Java programming language. The User gives input from the console and the output will be displayed in the console.
Sample Input:
4
AXZ
AXXZ
AYXYZ
AYZ

Sample output :
min star cost: 4
total cost: 11
A-X-Z
AXX-Z
AYXYZ
A-Y-Z

Sample Input 2:
3
AXZ
AY
A

Output:
min star cost: 3
total cost: 5
AXZ
A-Y
A--
