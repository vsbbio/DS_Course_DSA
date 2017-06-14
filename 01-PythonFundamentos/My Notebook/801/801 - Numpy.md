## [Numpy = Numeric Python]("http://www.numpy.org")

" To work with arrays and matrices"

## Arrays

### Creating

1. array = np.array([0,1,2,3,4], dtype=float64)
2. array2 = np.arange(start=0., stop=4.5, step=0.5)
3. array3 = np.zeros(10)
    3a. It creates an array of zeros (o.O)
4. array4 = np.eye(3)
    4a. It creates a matrice with 1 in the diagonal
5. array5 = np.diag(np.array([1,2,3,4])
    5a. It creates a matrice of the given numbers in the diagonal

### Object type, format and others attributes

1. type(array) => numpy.ndarray 
    1a. Type of the object
    
2. print(array.dtype) => float64, int32 (...)
    2a. Type of the elements inside the object. Watch out with the several types and its limitations  

3. np.shape(arrayname) "METHOD OF THE MODULE"
    3a. It returns/prints the shape of the array 
4. arrayname.shape "ATTRIBUTE OF THE OBJECT"


## Matrices

### Creating/Converting List in Arrays/Matrices

1. lst = [[0,1,2],[3,4,5],[6,7,8], dtype=float64"or int32, 64 (...)]
2. matriz = np.matrix(lst)
3. print(matriz):

    matrix( [0,1,2],
            [3,4,5],
            [6,7,8])

### Object type, format and others attributes

1. type(matriz) => numpy.matrixlib.defmatrix.matrix

2. matriz.size => 9

3. matriz.shape => (3,3) (rows, columns)

4. matriz.dtype => float64, int64 (...)

5. matriz.itemsize => 8 (bytes)
    5a. It returns the size in bytes of one item

6. matriz.nbytes => 72 (bytes)
    6a. It returns the total of bytes of the matrice 

7. matriz.ndim => 2
    7a. Number of matrix's dimension

### Other Functions

1. np.random.rand => To generate random numbers

2. np.loadtxt(filename, delimiter=",", usecols=(), skiprows=1) => To load a csv/txt file

3. np.mean(array) => It returns the mean (ôO)

4. np.std(array) => It returns the standard deviation

5. np.var(array) => It returns the variance

6. np.sum(array) => it returns the sum

7. np.prod(array) => It multiply all the numbers (Produtório)

8. np.cumsum(array) => It accumulate the sum in sequence

(...)
