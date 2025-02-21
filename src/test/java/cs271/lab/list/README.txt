COMP 313/413 Project 2

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


TestPerformance.java

	State how many times the tests were executed for each SIZE (10, 100, 1000 and 10000)
	to get the running time in milliseconds and how the test running times were recorded.
	These are examples of SIZEs you might choose, you can choose others if you wish.

	SIZE 10
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:  150  145  152  146   150 152  ... (fill these in in ms)
        testLinkedListAddRemove:  85 ms   80 ms  87 ms   82 ms   86 ms   83 ms  
        ArrayList Access           8 ms    7 ms    8 ms    7 ms    9 ms   8 ms   
        LinkedList Access          24 ms   23 ms   25 ms   22 ms   26 ms  24 ms  

	SIZE 100
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        ArrayList Add/Remove      | 280 ms | 275 ms | 290 ms | 285 ms | 278 ms | 272 ms 
        LinkedList Add/Remove     | 175 ms | 170 ms | 180 ms | 174 ms | 172 ms | 176 ms 
        ArrayList Access          | 10 ms  | 9 ms   | 11 ms  | 10 ms  | 12 ms  | 9 ms   
        LinkedList Access         | 75 ms  | 80 ms  | 85 ms  | 82 ms  | 77 ms  | 79 ms  

	SIZE 1000
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        ArrayList Add/Remove      | 450 ms | 470 ms | 460 ms | 455 ms | 465 ms | 458 ms 
        LinkedList Add/Remove     | 320 ms | 310 ms | 330 ms | 315 ms | 318 ms | 312 ms 
        ArrayList Access          | 15 ms  | 14 ms  | 16 ms  | 15 ms  | 17 ms  | 14 ms  
        LinkedList Access         | 350 ms | 360 ms | 370 ms | 355 ms | 365 ms | 358 ms 

	SIZE 10000
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:  1100 ms | 1080 ms | 1120 ms | 1095 ms | 1115 ms | 1105 ms 
        LinkedList Add/Remove     | 950 ms  | 970 ms  | 940 ms  | 960 ms  | 945 ms  | 955 ms  
        ArrayList Access          | 25 ms   | 24 ms   | 27 ms   | 26 ms   | 23 ms   | 25 ms   
        LinkedList Access         | 4500 ms | 4700 ms | 4600 ms | 4550 ms | 4680 ms | 4620 ms 