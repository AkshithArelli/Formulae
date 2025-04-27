**Return new array with elements**

return new array[] {ele1, ele2};

**Diff array and list**

arrays - fixed size
list - dynamic size

1D array: 

int[] array = new int[length];

2D array: 
int[][] 2darray = new int[][];

1D list:

List<Integer> list = new ArrayList<>();

2D list: (list of lists)
List<List<Intger>> 2dlist = new ArrayList<>();

**array of lists**
when array size is fixed but the values at each index is not fixed (if could be dynamic)

List<Integer>[] arrayOfLists = new int[5];
array of size 5. where each element of the array can store a list<Integer> (array size is fixed but elements length at each position is not fixed, then it is suggested to use array of lists)
eg: arrayOfLists = [[...], [...], [...], [...], [...]]
