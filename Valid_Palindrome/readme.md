https://leetcode.com/problems/valid-parentheses/description/

Approach
We use HashMap and Stack. We know valid combination, so initialize the combination with HashMap before we iterate through the input string.

mapping = { ")":"(", "}":"{", "]":"[" }
Stack has only open parentheses. When a close parenthesis comes, we use it as a key to find valid open parenthesis in the mapping. If the two parentheses(current parenthesis and the latest parenthesis in Stack) are not valid combination, we should return False.

At last, if Stack is empty, we should return True.
