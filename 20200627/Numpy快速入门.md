<a href="https://colab.research.google.com/github/liupengzhouyi/LearningColaboratory/blob/master/20200627/Numpy%E5%BF%AB%E9%80%9F%E5%85%A5%E9%97%A8.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

# Numpy 快速入门

## create Numpy Object


```python
import numpy as np
object0 = np.arange(1, 21)
print(object0)
```

    [ 1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20]


## create Numpy By function array()


```python
# list
object1 = np.array([1,2,3])
print(object1)
# tuple
object2 = np.array((2.2,3,4))
print(object2)
```

    [1 2 3]
    [2.2 3.  4. ]


## Setting Numpy Object Data Type When You Create Numpy Object


```python
object3 = np.array([123,456], dtype=np.float32)
print(type(object3))
print(object3.dtype)
```

    <class 'numpy.ndarray'>
    float32


## Create Zeros Numpy Object



```python
object4 = np.zeros((5, 7))
print(object4)
```

    [[0. 0. 0. 0. 0. 0. 0.]
     [0. 0. 0. 0. 0. 0. 0.]
     [0. 0. 0. 0. 0. 0. 0.]
     [0. 0. 0. 0. 0. 0. 0.]
     [0. 0. 0. 0. 0. 0. 0.]]


## create Ones Numpy Object


```python
object5 = np.ones((3, 4))
print(object5)
```

    [[1. 1. 1. 1.]
     [1. 1. 1. 1.]
     [1. 1. 1. 1.]]


## Create Range Numpy Object


```python
object6 = np.empty((3, 2, 4))
print(object6)
```

    [[[0.00000000e+000 2.32035990e+077 8.89318163e-323 0.00000000e+000]
      [2.12199579e-314 5.02034658e+175 4.08963275e-037 3.37923680e-057]]
    
     [[8.70404348e-071 3.72709079e-057 1.47763641e+248 1.16096346e-028]
      [7.69165785e+218 1.35617292e+248 1.48560457e+161 4.85637090e-033]]
    
     [[2.14297693e+160 2.67847530e-032 4.26489454e-096 6.32299154e+233]
      [6.48224638e+170 5.22411352e+257 5.74020278e+180 8.37174974e-144]]]


## Show Numpy Shape


```python
print(object6.shape)
```

    (3, 2, 4)


## change numpy shape


```python
object6 = object6.reshape(4, 6)
print(object6)
```

    [[0.00000000e+000 2.32035990e+077 8.89318163e-323 0.00000000e+000
      2.12199579e-314 5.02034658e+175]
     [4.08963275e-037 3.37923680e-057 8.70404348e-071 3.72709079e-057
      1.47763641e+248 1.16096346e-028]
     [7.69165785e+218 1.35617292e+248 1.48560457e+161 4.85637090e-033
      2.14297693e+160 2.67847530e-032]
     [4.26489454e-096 6.32299154e+233 6.48224638e+170 5.22411352e+257
      5.74020278e+180 8.37174974e-144]]


## Show Numpy Date Type


```python
# print(object0.dtype)
print(object0.dtype.name)
```

    int64


## Show Item Size


```python
print(object0.itemsize)
```

    8


## Show Numpy Object Size


```python
print(object0.size)
```

    20


## Show Object Type


```python
print(type(object0))
```

    <class 'numpy.ndarray'>


## List To Numpy


```python
tempList2 = list(range(1, 11))
print(tempList2)
newNumpyObject2 = np.array(tempList2)
print(newNumpyObject2)
print(type(newNumpyObject2))
```

    [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
    [ 1  2  3  4  5  6  7  8  9 10]
    <class 'numpy.ndarray'>


## Tuple To Numpy


```python
tempList1 = tuple(range(1, 11))
print(tempList1)
newNumpyObject1 = np.array(tempList1)
print(newNumpyObject1)
print(type(newNumpyObject1))
```

    (1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
    [ 1  2  3  4  5  6  7  8  9 10]
    <class 'numpy.ndarray'>


## Numpy Create Array

* return array type 


```python
object7 = np.arange(3)
print(object7)
print(object7.dtype)
```

    [0 1 2]
    int64

