Download Link: https://assignmentchef.com/product/solved-solved-a7-solved
<br>
(Quicksort) The recursive sorting technique called quicksort uses the following basic algorithm for a one-dimensional vector of values:

a) Partitioning Step: Take the first element of the unsorted vector and determine its final location in the sorted vector (i.e., all values to the left of the element in the vector are less than the element’s value, and all values to the right of the element in the vector are greater than the element’s value—we show how to do this below). We now have one value in its proper location and two unsorted subvectors.

b) Recursion Step: Perform the Partitioning Step on each unsorted subvector. Each time the Partitioning Step is performed on a subvector, another value is placed in its final location of the sorted vector, and two unsorted subvectors are created. When a subvector consists of one element, that element’s value is in its final location (because a one-element vector is already sorted).

The basic algorithm seems simple enough, but how do we determine the final position of the first element value of each subvector? As an example, consider the following set of values (the value in bold is for the partitioning element—it will be placed in its final location in the sorted vector):

37 2 6 4 89 8 10 12 68 45

Starting from the rightmost element of the vector, compare each element value with 37 until an element value less than 37 is found; then swap 37 and that element’s value. The first element value less than 37 is 12, so 37 and 12 are swapped. The new vector is

12 2 6 4 89 8 10 37 68 45

Element value 12 is in italics to indicate that it was just swapped with 37. Starting from the left of the vector, but beginning with the element value after 12, compare each element value with 37 until an element value greater than 37 is found— then swap 37 and that element value. The first element value greater than 37 is 89, so 37 and 89 are swapped. The new vector is

12 2 6 4 37 8 10 89 68 45

Starting from the right, but beginning with the element value before 89, compare each element value with 37 until an element value less than 37 is found—then swap 37 and that element value. The first element value less than 37 is 10, so 37 and 10 are swapped. The new vector is

12 2 6 4 10 8 37 89 68 45

Starting from the left, but beginning with the element value after 10, compare each element value with 37 until an element value greater than 37 is found—then swap 37 and that element value. There are no more element values greater than 37, so when we compare 37 with itself, we know that 37 has been placed in its final location of the sorted vector. Every value to the left of 37 is smaller than it, and every value to the right of 37 is larger than it. Once the partition has been applied on the previous vector, there are two unsorted subvectors. The subvector with values less than 37 contains 12, 2, 6, 4, 10 and 8. The subvector with values greater than 37 contains 89, 68 and 45. The sort continues recursively, with both subvectors being partitioned in the same manner as the original vector.

Based on the preceding discussion, write a recursive function, quickSortHelper, to sort ten one-dimensional integer vectors. The function should receive as arguments a starting index and an ending index on the original vector being sorted. Please create ten vectors with random size from 0 ~20 elements and randomly choose the size of the vector numbers from 0~100. Put the numbers in the vectors and use quick sort to sort them.

This assignment comes with a CISP400V9A7.zip file. It includes CISP400V9A7.exe file. The CISP400V9A7.exe file is an executable file. You can double click the file to get to the expecting result of this assignment.

The following are some of the displays of the expecting results.

Please be aware the vector size is randomly choose from 0 ~ 20 and the created sized for a vector is listed inside a pair of parentheses (“ ( )”).

Please be aware that the display of the vector size equals to zero and one are different from the size greater than and equal to 2.

Please document all your files properly and zip all your files into a proper named zip file for this assignment (refer to the assignment section of the class syllabus) and submit it to the A7 dropbox of the D2L Website.

Worth 150 points

AD7

Our linked list class template allowed insertions and deletions at only the front and the back of the linked list. These capabilities were convenient for us when we used private inheritance and composition to produce a stack class template and a queue class template with a minimal amount of code by reusing the list class template. Actually, linked lists can do more than those provided by the textbook. In this assignment we want to have a linked list class template to handle insertions and deletions anywhere in the list.

Modify Fig. 19.4(ListNote.h) and Fig19.5(List.h) to work with a driver to create an interface to add anywhere in the list , delete a particular element, repopulate the list and exit the list. The program will populate a 20 elements integer list with random number from 0 ~ 200. The list can expend to more than 100 and shrink to 0 element.

This assignment comes with a CISP400V9AD7.zip file. It includes CISP400V9AD7.exe file. The CISP400V9AD7.exe file is an executable file. You can double click the file to get to the expecting result (see the picture below) of this assignment. After you finish modifying ListNote.h and List.h and create CISP400V9AD7.cpp file you can put them in a project and run to the exe file result.

The following are some of the displays of the expecting results.

The right side of picture is a display of a starting of the program. The list contains 20 numbers which is in between 0 and 200.

We should get a different list of data every time we start the program.

We should be able to Exit the program any point when -1 is entered at a selection menu.

The program should allow you to insert a number in between index 0 to number of numbers in the list.

You can randomly delete any number on the list.

After we deleted all the number on the list, the screen should display “The list is empty” information.

When we delete a number but there is more than one occurrence of the number in the list, the lower order (index) number will be deleted.

When we delete an item but there is no occurrence in the list, there should show “The number is not found.” Information.

At any point, a user can choose third option of the menu item to generate a new 20 numbers list.

At the menu selection, if a user chooses a number other than -1, 1, 2 and 3, the program should display an error message and allows the user to reenter a selection.

Please document CISP400V9AD7.cpp, ListNote.h and List.h files properly and zip them into a proper named zip file for an advance assignment (refer to the assignment section of the class syllabus) and submit it to the A7 dropbox of the D2L Website.

Worth 180 points