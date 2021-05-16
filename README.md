
**Algorithms**
@ Prof. Sampath Kannan, Prof. Arvind Bhusnurmath  from Penn
```Java
@ Note by Gary Zhang
```

- Create and analyze the paradigms of divide-and-conquer, randomized algorithms, greedy algorithms, and dynamic programming
- Distinguish important and basic algorithms for sorting and selection and create new algorithms using these
- Describe basic graph algorithms, including network flow, and utilize them in solving new problems
- Differentiate the complexity classes P, NP, and NP-complete, and be able to show problems NP-complete

[Syllabus](https://d18ky98rnyall9.cloudfront.net/12rr2CVKSXKq69glSmly7A_cb4355cbe7c943ed8a75a072a6cbfaf1_CIT-596---Syllabus---Summer-2021_v2.pdf?Expires=1621296000&Signature=Ktp0kdZXxblgpDr4h5fbRC5OLhXHkICi~f-HxMMO4lMr7HQVJFXxbVCr8vYdotKPMC5EzdBStO6F~MEo-lYcLNSMvLACFiVP13LuBrvF-WmAFVUkogtrFoxo42ZLGCBLQrFwRyx-CAgAOkso3b0IJzbMGqyAF70Q-GPwEcPGqoY_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)

- 14 Quick Quizzes: 10%
- 7 Individual Assignments: 55%
- Midterm 1 (M1-M5): 10%
- Midterm 2 (M6-M10): 10%
- Final (Cumulative, but more on M11-M14): 15%

## M1: Intro. Algorithms

The first module of this course begins by situating the study of algorithms on a mathematical base, supplemented by an interview with Professor Sanjeev Khanna. We use the example of creating a simple algorithm, and then improving upon it, to gain insight into foundational algorithm analysis. It also covers how we argue that algorithms are correct, emphasizing the course motto “Correctness first, then efficiency.” This module also overviews the logistics and policies for this course.

Learning Objectives
- Summarize the algorithms for max-subinterval sum.
- Analyze the running time of nested loop code fragments.
- Explain how to use asymptotic 渐进 notation and asymptotic analysis.

### Model of Computation
Asymptotics: Growth rate of functions without regard to constants

* Worst-case complexity：growth rate of function $f(n)$ is max time algorithm takes on any input of length n
* **Big-Oh**: $\leq$ upper bound 
    * $f(𝑛) = O(g(n))$ if $f(𝑛) \leq k g(n)$ for $n \geq n_0$ for connstants $k, n_0$
    * $f(n)$ grows no faster than $g(n)$
    * little oh: $lim_{n \rightarrow \infty}  \frac{f(n)}{g(n)}=0$
        * $log(n)= o(n)$<br>
        $lim_{n \rightarrow \infty} \frac{log(n)}{n}= lim_{n \rightarrow \infty} \frac{1/n}{1}=0$
* **Big-Omega**: $\geq$ lower bound
    * $g(𝑛) = \Omega(f(n))$ if $g(𝑛) \geq k f(n)$ for $n \geq n_0$ for connstants $k, n_0$
    * $g(n)$ grows no slower than $f(n)$
    * ! Lower bounds are also for the worst case!
* **tight bound**:
    * If we have an upper bound $f(n)$ and lower bound $g(n)$ on an algorithm’s running time and $f(n)=O(g(n))$ then we have a tight bound, We say the algorithm runs in time $\theta(f(n))$ in this case
    * $f(n)= \theta(g(n))$ if $k_1g(n) \leq f(n) \leq k_2g(n)$

### Subinterval of Maximum Sum

### Leetcode
#### 53 Maximum Subarray

#### 309 Best Time to buy and sell stock with Cooldown


## M2: Designing Algorithms inductively and recursively

Module 2 introduces summing series, a useful tool throughout the course, and two examples that illustrate the main ways of designing algorithms, InsertionSort and Towers of Hanoi. InsertionSort is an algorithm that results from thinking inductively, while Towers of Hanoi illustrates thinking recursively. We go over how to solve the “recurrence relation” that governs the running time of a recursive algorithm. Finally, the module covers Euclid’s classic algorithm for computing GCD (greatest common divisor.)

Learning Objectives
- Apply computing sums of series.
- Explain the Insertion Sort algorithm and its analysis.
- Explain the Towers of Hanoi algorithm and its analysis.
- Examine Euclid's algorithm for finding the GCD.

### Leetcode
#### 147 Insertion Sort List

#### 1071 Greatest Common Divisor of Strings

## M3: Divide-and-Conquer Algorithms

This module introduces “divide-and-conquer” algorithms, which break up the problem you want to solve into “divide,” “conquer,” and “combine” steps. It illustrates a real use of this paradigm using the MergeSort algorithm. This module also covers how to solve recurrence relations, and proves the Master Theorem. Finally, this module introduces a useful variation of the divide-and-conquer paradigm, often referred to as "decrease-and-conquer" where at each step you generate only one subproblem.

Learning Objectives
- Describe the MergeSort algorithm.
- Use the Master Theorem for solving recurrences.
- Create Divide-and-Conquer algorithms for new problems.
- Inspect the runtime of divide-and-conquer algorithms.

## M4: Randomized Algorithms: Sorting and Selection

This module gives a brief review of probability, before introducing the concepts of randomized algorithms and designing algorithms for sorting and selection. Our primary focus will be analyzing two widely used randomized algorithms, QuickSort and QuickSelect. We will also discuss a way to remove randomization from QuickSelect, and briefly touch upon analyzing the lower bounds of comparison-based algorithms.

Learning Objectives
- Discuss the coupon collector analysis.
- Summarize binary search analysis.
- Create correct and efficient algorithms based on sorting.
- Compare the analyses of QuickSort and QuickSelect.
- Understand deterministic linear-time selection.
- Understand random variables, and expectations and analysis of randomized algorithms.

## M5: Data Structure

This module will review some important data structures that you may have seen in previous courses. These include heaps, binary search trees, and hash tables. The last two are specific implementations of a general data structure called the dictionary. We will also see a more efficient version of the binary search tree called the balanced binary search tree that guarantees good worst-case behavior on dictionary operations. We will analyze these data structures as well as explore some modifications we can make to them to expand their capabilities.

Learning Objectives
- Evaluate the best data structure for a particular application.
- Describe Binary Search Trees.
- Define heaps and their uses.
- Examine algorithms that use these data structures (Heaps, Binary Search Trees and Hash Tables.)
- Prepare algorithms using these data structures (Heaps, Binary Search Trees and Hash Tables.)
- Understand Hash Tables.

## M6: Graphs and Graph Traversals

This module reviews the basics of graphs and graph terminology and then explores efficient representations of graphs in computers. Then, two of the classic graph algorithms, depth-first search and breadth-first search, are introduced. We finish with two applications of depth-first search: the topological sorting algorithm and an algorithm for finding the strongly connected components of a directed graph.

Learning Objectives
- Understand and describe the Depth-First Search algorithm.
- Describe the applications of Depth-First Search and Breadth-First Search.
- Understand and describe the Breadth-First Search algorithm.
- Create correct algorithms for new problems using Depth-First Search and Breadth-First Search.

## M7: Greedy Algorithms

This module introduces the idea of optimization problems and explores a particular approach to such problems: greedy algorithms. We will explore when such algorithms are applicable, and if so, how to prove they are correct. As examples, we will show two canonical problems: job scheduling and interval scheduling. The module closes by analyzing Huffman Coding, a data compression scheme which uses a greedy algorithm.

Learning Objectives
- Discuss the particular examples of greedy algorithms shown.
- Test greedy algorithms to prove they work.
- Judge whether a problem can be solved by a greedy algorithm.
- Understand basic terminology about optimization problems.
- Understand the Exchange and Progress arguments to prove correctness of greedy algorithms.
- Create correct greedy algorithms for new problems.
- Explain the concept of greedy algorithms.

## M8: Spanning Trees and Shortest Paths - Greedy Algorithms

In this module, we focus on using greedy algorithms for graph problems. The module covers finding minimum spanning trees, particularly covering two classic algorithms, Kruskal’s and Prim’s algorithms. It also covers another type of greedy algorithm, “single-source shortest paths” to find the shortest paths from a starting point to all other points in a graph, in particular highlighting Dijkstra’s algorithm.

- Describe Kruskal’s and Prim’s Algorithms for minimum spanning trees.
- Develop proofs of new theorems about MSTs and Shortest Paths.
- Understand the Graph-Theoretic Properties needed for proving correctness of MST algorithms.
- Describe Dijkstra’s Algorithm for single-source shortest paths.
- Judge whether a problem can be solved by a greedy algorithm.

## M9-10: Dynamic Programming

The topic for M9 is dynamic programming: a paradigm for algorithm design built from a series of potential decisions and trying all their possibilities. The first segment uses this paradigm to solve the weighted activity selection problem, and the second gives another example: optimizing a railway route for commuter accessibility. We finish by covering sequence alignment, and presenting a dynamic programming algorithm for counting paths in a graph. Along with way, we have an interview with Prof. Junhyong Kim, a professor of Biology at Penn, and a frequent collaborator with computer scientists.

M9 Learning Objectives
- Explain the concept of Dynamic Programming.
- Create dynamic programming algorithms for new problems.
- Analyze dynamic programming algorithms for correctness and run-time.
- Summarize the particular examples of dynamic programming used in this module.
- Describe the importance of the Sequence Alignment problem in other fields.
- Describe the main steps in designing dynamic programming algorithms.

M10 continues our exploration of dynamic programming, highlighting optimal static binary search trees and finding the shortest paths between pairs of vertices. Several algorithms that solve the shortest path problem are covered, including the Floyd-Warshall algorithm and the Bellman-Ford algorithm. The module also discusses another key problem, the segmented regression problem, and features a fun interview with Dr. Boulos Harb, a senior staff scientist at Google.

M10 Learning Objectives
- Judge which shortest path algorithm is best in various situations.
- Describe the Floyd-Warshall Algorithm.
- Explain linear regression and piecewise linear regression.
- Describe the Bellman-Ford Algorithm.
- Explain the matrix-multiplication-based shortest path algorithm.
- Develop complex dynamic programming algorithms for new problems.
- Analyze any dynamic programming algorithm.

## M11: Network Flows

This module covers the problem of finding maximum flows in networks--one that doesn’t fall into any paradigms covered in previous models. Instead, it explores an iterative build-up of the solution. Both this approach and the underlying theory are very important in studying many optimization problems. We cover the Ford-Fulkerson algorithm for solving the max flow problem and prove its correctness, and then close by showing how the max flow problem can be applied to matchings in bipartite graphs.

Learning Objectives
- Explain the Max-flow-min-cut theorem.
- Create algorithms for new problems using the max flow algorithm.
- Understand the Ford-Fulkerson algorithm and analysis.
- Develop proofs of new theorems about properties of flows.
- Interpret the Network Flow problem.
- Discuss how to use network flow to solve bipartite matching.

## M12: Intro. Computational Complexity - P, NP, NP-Complete

This module steps back from specific problems to understand the general theory of what it means to have efficient algorithms. It focuses on decision problems, including a class of decision problems called NP, standing for non-deterministic polynomial time. It explores whether we can solve problems in NP in polynomial time, highlighting a famous question in computer science: is P equal to NP? To approach this question, we first need to understand the “hardest problems” in NP, called NP-complete problems, by using the concept of polynomial-time reductions.

Learning Objectives
- Understand the class NP.
- Define the class NP-complete.
- Understand the class P.
- Discuss Boolean circuits from a theoretical perspective.
- Formulate basic reductions from search problems to decision problems.
- Explain the concept of polynomial-time reductions.

## M13: Cook-Levin Theorem and First NP-Complete Problems

In this module we prove the Cook-Levin Theorem, which shows that the problem of Satisfiability is NP-complete. We do this by defining Boolean circuits and showing that the problem of Circuit-Satisfiability is NP-complete. The module reviews Boolean algebra and Boolean logic from CIT 593 to help prove the NP-completeness of these problems. The module closes by demonstrating an example of a reduction, which shows that the Independent Set problem in graphs is NP-complete.

Learning Objectives
- Apply the above ideas to new problems.
- Demonstrate the NP-completeness of Satisfiability and 3-SAT.
- Understand reductions formally.
- Explain Boolean circuits as computers.
- Describe the reduction from 3SAT to Independent Set.
- Describe the Cook-Levin Theorem.

## M14: Reductions to show NP-Completeness, Wrapping Up

In the final module, we look at the variety of different problems that have been shown to be NP-complete. These include the 3-coloring problem, vertex cover and clique. We also show a number problem called subset sum NP-complete with a more complicated reduction. The module finishes by summarizing the large amount of material this course covered, the techniques for algorithm design you will now have in your toolkit, and how you can cope with NP-completeness in practice.

Learning Objectives
- Interpret proofs of NP-completeness of classic NP-complete problems such as 3-coloring, vertex cover, and subset sum.
- Develop correct reductions showing new problems NP-complete
- Recall major concepts covered in the course.
- Summarize the definition of an approximation algorithm.
- Evaluate the correctness of a reduction argument.
