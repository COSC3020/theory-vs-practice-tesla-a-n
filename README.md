# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.
    1. Constant factors and lower order terms are ignored when considering asymptotic
       complexity so in practice, the complexity might perform worse for smaller input
       sizes because of those high constant factors. Within this the overhead time is
       also ignored because it might take more time if the data structure needs to be
       implemented or the algorithm needs more work to be implemented
    2. Different hardwares create environments that may optimize/hurt an algorithms
       performance. Some algorithms may take advantage of the systems it's offered and
       others may not. Examples of hardware features that influence time could be
       different architectures, runtime environments, or compilers.
    3. Extending off the influence of hardware would be how well the algorithm uses
       the hardware it's supposed to use like memory and cache. If the algorithm isn't
       using memory as well as it could it's not as fast as the algorithm could be.
       Excessive use of memory or cache misses would affect the complexity without
       there being an issue with the methods of the algorithm.
https://www.sciencedirect.com/topics/computer-science/asymptotic-complexity

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

Add your answers to this markdown file.
