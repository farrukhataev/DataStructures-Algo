function logItems(n) {
    for(let i = 0; i < n; i++) {
        console.log(i)
    }
}

logItems(10) --> Runs 10 times (prints 0 to 9)

##
Big O of n  simply means that the time or number of steps your code takes grows directly in proportion to the size of the input (\(n\)).

Think of it like reading a book page by page:

If a book has 10 pages, you do 10 steps (flip 10 pages)

If a book has 1,000 pages, you do 1,000 steps.

n is the number you pass into the function.
The for loop does one piece of work (console.log) for each number up to n.
If you pass 10, it runs 10 times.
 If you pass 100, it runs 100 times.

 In \(O(n)\) (also called Linear Time), the workload scales in a straight line: double the input, double the work.