# Comp110 Worksheet 5
## Cole Gilbert

### A
The algorithm will check through a list to determine if there is a duplicate of an item within the list by checking each item in the list against each item in the list, apart from itself.

### B
The worst case running time of the algorithm is quadratic because for each time the algorithm runs, line 4's for loop iterates for each element in the list, meaning that for every element in the list, the whole list iterates, meaning that in order to finish determining if there are duplicates in the list, the algorithm goes through the list an amount of times equal to O(n)*O(n), or O(n^2).

### C
The algorithm is still correct because each element of the list is still checked against each other element, this occurs because every item in the list is checked against every item that comes before it in the list, therefore eventually once the end of the list has been reached, every item has been checked against every other item.

### D
The algorithm will run approximately twice as fast because on average over the course of the algorithm the average elements that are checked from the list on line 4 is roughly half the length of the list. This is because for the first half of the list, less than half of all the elements are being compared to each other, and then for the second half, more than half of all the elements are being compared. Resulting in about half the time required to compare all of the items.

### E
The time complexity is still quadratic because the list is still being iterated through in two different for loops, meaning that the list still has to be compared through twice, resulting in O(n)*O(n) which is simplified to O(n^2). Therefore, it is still quadratic.

### F
https://wiki.python.org/moin/TimeComplexity Python's wiki shows the time complexity for average and worst cases of functions in the language. On the page, it shoes that the sort() function has a time complexity of O(n log n) for both average and worst cases.

### G
Because the algorithm uses the python sort() function, it inherits the time complexity of O(n log n) because that is the time complexity in which the sorting of the algorithm is operating. 

### H
The second algorithm will run faster because O(n log n) runs the algorithm in less operations than the first algorithm in which the time complexity is O(n^2). This happens because the operations required with O(n^2) increases exponentionally with the increase in elements of the list. Whereas the growth for O(n log n) is less steep and therefore will be able to complete the algorithm sooner.

### I
You might choose to use the slower algorithm in this case because it doesn't deal with sorting the list, meaning that the algorithm might actually complete faster for smaller sized lists as it doesn't require additional steps in order to start comparing elements. This would be more visible in a best case scenario in which the procedure finds a duplicate early on, perhaps whilst the 'faster' algorithm is finishing sorting and moving in to comparisons.
