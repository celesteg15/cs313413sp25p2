Conduct the performance measurements: you will find the running times in the test report.
Create a new doc folder in the project.
Create a document called README.txt in doc and answer the various TODO Questions embedded in the code.


TestIterator:
  // TODO Question: Also try with a LinkedList - does it make any difference?
    Yes, LinkedList are slower than ArrayList due to factors like node traversal

 // TODO Question: What happens if you use list.remove(Integer.valueOf(77))? 
  the first 77 encountered is removed


TestList:

TODO Question: Also try with a LinkedList - does it make any difference?
    Yes! LinkedList removal/addition in the middle is faster, but access is slower compared to ArrayList

TODO Question: What does this method do? Gets rid of element @ index of 5 NOt the value 5

TODO Question: What does this one do? Removes the first submission of the value 5


TestPerformance:

TODO Question: What conclusions can you draw about the performance of LinkedList vs. ArrayList when
comparing their running times for AddRemove vs. Access? Record those running times in README.txt!

    Add/Remove -> LinkedList is faster when adding/removing at the start/middle due to O(1) pointer updates.
    ArrayList is slower for middle insertions/removals due to O(n) shifting.
    Access:

    ArrayList = (O(1)) since it uses indexed access.
    LinkedList = (O(n)) as it requires traversing nodes.

Test method runtimes:
2s, 1s, 2s, 1s