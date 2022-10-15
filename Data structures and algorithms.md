
# Data structures and algorithms study cheatsheets for coding interviews

## What is this[​](#what-is-this "Direct link to heading")

This section dives deep into practical knowledge and techniques for algorithms and data structures which appear frequently in algorithm interviews. The more techniques you have in your arsenal(武器库), the higher the chances of passing the interview. They may lead you to discover corner cases you might have missed out or even lead you towards the optimal approach!

## Contents of each study guide[​](#contents-of-each-study-guide "Direct link to heading")

For each topic, you can expect to find:

1.  A brief overview
2.  Learning resources
3.  Language-specific libraries to use
4.  Time complexities cheatsheet
5.  Things to look out for during interviews
6.  Corner cases
7.  Useful techniques with recommended questions to practice

## Study guides list[​](#study-guides-list "Direct link to heading")

Here is the list of data structures and algorithms you should prepare for coding interviews and their corresponding study guides:

Topic


## General interview tips[​](#general-interview-tips "Direct link to heading")

Clarify(理清) any assumptions(假设) you made subconsciously(下意识地). Many questions are under-specified(明确) on purpose(目标).

Always validate input first. Check for invalid/empty/negative/different type input. Never assume(假设) you are given the valid parameters. Alternatively(或者), clarify with the interviewer whether you can assume valid input (usually yes), which can save you time from writing code that does input validation.

Are there any time/space complexity requirements/constraints(约束)?

Check for off-by-one errors.

In languages where there are no automatic type coercion(强制转换), check that concatenation of values are of the same type: `int`/`str`/`list`.

After finishing your code, use a few example inputs to test your solution.

Is the algorithm meant to be run multiple times, for example in a web server? If yes, the input is likely to be preprocess-able to improve the efficiency in each call.

Use a mix of functional and imperative(效率) programming paradigms:

*   Write pure functions as much as possible.
*   Pure functions are easier to reason about and can help to reduce bugs in your implementation.
*   Avoid(防止) mutating the parameters passed into your function especially if they are passed by reference unless you are sure of what you are doing.
*   However, functional programming is usually expensive in terms of space complexity because of non-mutation and the repeated allocation of new objects. On the other hand, imperative code is faster because you operate on existing objects. Hence you will need to achieve a balance between accuracy vs efficiency, by using the right amount of functional and imperative code where appropriate.
*   Avoid relying on and mutating global variables. Global variables introduce state.
*   If you have to rely on global variables, make sure that you do not mutate it by accident.

Generally, to improve the speed of a program, we can either: (1) choose a more appropriate data structure/algorithm; or (2) use more memory. The latter demonstrates a classic space vs. time tradeoff, but it is not necessarily the case that you can only achieve better speed at the expense of space. Also, note that there is often a theoretical limit to how fast your program can run (in terms of time complexity). For instance, a question that requires you to find the smallest/largest element in an unsorted array cannot run faster than O(N).

Data structures are your weapons. Choosing the right weapon for the right battle is the key to victory. Be very familiar about the strengths of each data structure and the time complexities for its various operations.

Data structures can be augmented to achieve efficient time complexities across different operations. For example, a hash map can be used together with a doubly-linked list to achieve O(1) time complexity for both the `get` and `put` operation in an [LRU cache](https://leetcode.com/problems/lru-cache/).

Hash table is probably the most commonly used data structure for algorithm questions. If you are stuck on a question, your last resort can be to enumerate through the common possible data structures (thankfully there aren't that many of them) and consider whether each of them can be applied to the problem. This has worked for me sometimes.

If you are cutting corners in your code, state that out loud to your interviewer and say what you would do in a non-interview setting (no time constraints). E.g., I would write a regex to parse this string rather than using `split()` which may not cover all cases.

[

**Stop grinding mindlessly. Study with a plan**Developed by Google engineers, AlgoMonster is the fastest way to get a software engineering job. Check it out for free!

](https://shareasale.com/r.cfm?b=1873647&u=3114753&m=114505&urllink=&afftrack=)

Recommended courses[​](#recommended-courses "Direct link to heading")
---------------------------------------------------------------------

### [AlgoMonster](https://shareasale.com/r.cfm?b=1873647&u=3114753&m=114505&urllink=&afftrack=)[​](#algomonster "Direct link to heading")

AlgoMonster aims to help you ace the technical interview **in the shortest time possible**. By Google engineers, AlgoMonster uses a data-driven approach to teach you the most useful key question patterns and has contents to help you quickly revise basic data structures and algorithms. Best of all, AlgoMonster is not subscription-based - pay a one-time fee and get **lifetime access**. [**Join today for a 70% discount →**](https://shareasale.com/r.cfm?b=1873647&u=3114753&m=114505&urllink=&afftrack=)

### [Grokking the Coding Interview: Patterns for Coding Questions](https://designgurus.org/link/kJSIoU?url=https%3A%2F%2Fdesigngurus.org%2Fcourse%3Fcourseid%3Dgrokking-the-coding-interview)[​](#grokking-the-coding-interview-patterns-for-coding-questions "Direct link to heading")

This course on by Design Gurus expands upon the questions on the recommended practice questions but approaches the practicing from a questions pattern perspective, which is an approach I also agree with for learning and have personally used to get better at coding interviews. The course allows you to practice selected questions in Java, Python, C++, JavaScript and also provides sample solutions in those languages along with step-by-step visualizations. **Learn and understand patterns, not memorize answers!** [**Get lifetime access now →**](https://designgurus.org/link/kJSIoU?url=https%3A%2F%2Fdesigngurus.org%2Fcourse%3Fcourseid%3Dgrokking-the-coding-interview)

### [Master the Coding Interview: Data Structures + Algorithms](https://fxo.co/DQpY)[​](#master-the-coding-interview-data-structures--algorithms "Direct link to heading")

This Udemy bestseller is one of the highest-rated interview preparation course (4.6 stars, 21.5k ratings, 135k students) and packs **19 hours** worth of contents into it. Like Tech Interview Handbook, it goes beyond coding interviews and covers resume, non-technical interviews, negotiations. It's an all-in-one package! Note that JavaScript is being used for the coding demos. [**Check it out →**](https://fxo.co/DQpY)
