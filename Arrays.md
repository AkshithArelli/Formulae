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

List<Integer>[] arrayOfLists = new List[5];
array of size 5. where each element of the array can store a list<Integer> (array size is fixed but elements length at each position is not fixed, then it is suggested to use array of lists)
eg: arrayOfLists = [[...], [...], [...], [...], [...]]



2D Matrix
eg:
int[][] matrix = {
          {1,2,3},
          {4,5,6}
}

no.of rows = matrix.length //2
no.of columns = matrix[0].length //3

matrix[i][j] //access element at ith row and jth column

Iterate through a matrix

for (int i=0; i<matrix.length; i++) {
  for (int j=0; j<matrix.length; j++) {
  }
}





