What is Big O?

Big O, also known as Big O notation, represents an algorithm's worst-case complexity. It uses algebraic terms to describe the complexity of an algorithm.

Big O defines the runtime required to execute an algorithm by identifying how the performance of your algorithm will change as the input size grows. But it does not tell you how fast your algorithm's runtime is.

Big O notation measures the efficiency and performance of your algorithm using time and space complexity.

Why is time complexity a function of its input size?
To perfectly grasp the concept of "as a function of input size," imagine you have an algorithm that computes the sum of numbers based on your input. If your input is 4, it will add 1+2+3+4 to output 10; if your input is 5, it will output 15 (meaning 1+2+3+4+5).


###
const calculateSum = (input) => {
  let sum = 0;       ------> Statement 1
  for (let i = 0; i <= input; i++) {
    sum += i;        ------> Statement 2
  }
  return sum;        ------> Statement 3
};
###


Looking at the image above, we only have three statements. Still, because there is a loop, the second statement will be executed based on the input size, so if the input is four, the second statement (statement 2) will be executed four times, meaning the entire algorithm will run six (4 + 2) times.

In plain terms, the algorithm will run input + 2 times, where input can be any number. This shows that it's expressed in terms of the input. In other words, it is a function of the input size.
 ##
In Big O, there are six major types of complexities (time and space):

Constant: O(1)

Linear time: O(n)

Logarithmic time: O(n log n)

Quadratic time: O(n^2)

Exponential time: O(2^n)

Factorial time: O(n!)
##


The Big O chart above shows that O(1), which stands for constant time complexity, is the best. This implies that your algorithm processes only one statement without any iteration. Then there's O(log n), which is good, and others like it, as shown below:

O(1) - Excellent/Best

O(log n) - Good

O(n) - Fair

O(n log n) - Bad

O(n^2), O(2^n) and O(n!) - Horrible/Worst