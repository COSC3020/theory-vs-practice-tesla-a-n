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
Source: https://www.sciencedirect.com/topics/computer-science/asymptotic-complexity

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.
    Since the search time is logarithmic, we can find the increase in search
    time by finding the proportion of searching 1000 elements to 10000 elements.
      log(1000) is about 10
      log(10000) is about 13.3
      Their ratio is 13.3/10 = 1.33
    The search time for 10,000 is about 1.33 longer than the search with 1,000
    elements so we then apply that to the search time for 10000 elements : 5 x 1.33
    is about 6.65 seconds
Source: ChatGPT provided instructions on how to calculate complexity and multitudes
 of performance. 
- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.
    If a search with 10,000 elements takes 100 seconds and asymptotic complexity
  suggests a much better time, an inefficient stucture or balance in the tree or
  high overhead and poor data usage may also be to blame. Unbalanced trees are
  best avoided due to their effect on search time because it takes the time
  complexity from logarithmic to linear ( O(logn) to O(n) ). If a tree has most
  elements on one side of a tree the search becomes similar to searching through
  a list becasue it lacks the branches that are beneficial in complete BST.
    Another way inefficient structure may increase search time is if the nodes
  have poor structure. The nodes could have poor memory placement or complex
  pointers to the next node which increases search time when each traversal
  is complex and could easily be missed and give extra overhead per node.
    If the BST doesn't have many issues itself, the environment or language it
  is implemented in may effect performance. From using pointers in C or C++,
  some languages offer more control over memory allocation than languages
  like Python or Java that have managed memories which handle memory automatically
  which can be inefficient at times.
      Source: https://en.wikipedia.org/wiki/Binary_search_tree
  Add your answers to this markdown file.

  "I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice."
