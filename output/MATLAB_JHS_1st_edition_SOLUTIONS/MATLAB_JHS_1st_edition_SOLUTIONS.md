7–196 Arrays

## **Problem 7-A.8**

Write a function, **Prob5**, that takes one array input and produces one array output. Internally, your function should construct the single output array with elements taken from the input array, specifically from the third and fourth rows and from the last five columns of the input array. Assume that the input array has dimensions n x m such that n>4, and m>5. In your indexing solution, use **end**.

```
function selectRegion = Prob5(anArray)
% returns an array that consists of the 3rd and 4th rows 
% in the last 5 columns of the input array
% INPUT: An n by m array where n >= 4 and m >= 5
% OUTPUT: A 2 by 5 array 
selectRegion = anArray(3:4,end-4:end);
```

## **Problem 7-A.9**

Write a function, **Prob7\_A\_9**, that takes one array input and produces one array output. Internally, your function should set the last four elements in the first row of the input to 2 and return the modified array. Assume that the input array has dimensions n x m such that m>3.

```
function anArray = Prob7_A_9(anArray)
% sets the last four elements in the first row of the input
% array to 2
% INPUT: An n by m array where m >= 4
% OUTPUT: The modified n by m array
anArray(1,end-3:end)=2;
```