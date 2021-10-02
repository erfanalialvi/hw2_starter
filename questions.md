# HW2 Questions
## UMBC CMSC 671 fall 2021

Please answer the following questions using the git [markdown syntax](https://guides.github.com/features/mastering-markdown/).  You should view this file on your repo on GitHub after pushing it to make sure it looks the way you want.  You can also use a browser extension (like [this one](https://chrome.google.com/webstore/detail/markdown-preview-plus/febilkbfcbhebfnokafefeacimjdckgl) for Chrome) to view your local file.

### (1) Describe in words the heuristic you used for the steps cost and explain why it is admissable

The heuristic I used is the difference in no. of characters in my current state from goal state. For example: if my current state is DOG and goal is CAT then all 3 characters are different, so my heuristic will return 3. If my state is CAG and the goal is CAT, then only one letter needs to be changed so my heuristic will return 1. It is admissible because it will never overestimate the cost, as it calculates cost in unit steps.

### (2) Describe in words the heuristic you used for the scrabble cost and explain why it is admissable
I used the same heuristic that calculates the difference in no. of characters in my current state from goal state. It is admissible because the minimum cost in scrabble rules is 1 and so does my heuristic calculates in unit steps, hence it will never overestimate the cost.

### (3) Describe in words the heuristic you used for the frequency cost and explain why it is admissable

I used the same heuristic that calculates the difference in no. of characters in my current state from goal state. It is admissible because the minimum cost in frequency rules is always greater than 1 (1 +R) and so does my heuristic calculates in unit steps, hence it will never overestimate the cost.

### (4) Given an intiial word W1 and goal words W2, if there is a shortest path with N steps from W1 to W2, will there also be a shortest path of N steps from W2 to W1?  Explain why or why not.

Yes, because if the alphabets are replaced in the reverse order from W2 to W1, I can reach back to W1 in exact same number of steps. For example: if I  can go from  DOG--> DOT --> DAT --> CAT, I can also traverse CAT --> DAT--> DOT --> DOG. In other words, if W2 is reachable from W1 in N steps, W1 is also reachable from W2 in N steps.

### (5) Using the steps cost, what is the longest path for a pair of three- and four-letter words you can find?

I think it will be equal to the meaningful words in the dictionary, so it might be 90 steps
