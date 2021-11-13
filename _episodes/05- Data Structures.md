---
title: " Intoduction to data structures"
questions:
- "Key question (FIXME)"
objectives:
- " understanding different data structure"
- "learn about functions of each data structure"

keypoints:
- "understanding difference between data structures"
---
FIXME

### **1. VECTORS**
Vectors are the basic data structure of R. Vectors can hold multiple values together using the concatenate **c()** function. 
The type of data inside a vector can be determined by using **typeof()** function and the length (or)
number of elements in a vector can be found with **length()** function. 

R uses one indexing, hence the position of the first component in a vector can be accessed by,**vector_name[1]**

[FIXME add code image]

A vector will **always** contain data of same data type. If a vector contains multiple data types 
the vector will convert all its values to the same data type in the below order of precedence: 

• Character 

• Double (Float / Decimals) 

• Integers (Round whole numbers)

[FIXME add code image for each data type]

#### **Analyzing a Vector**

class(vector_name) - Type of data present inside the vector 

str(vector_name) - Structure of the vector 

is.na(vector_name) - Checks if each element of vector is “NA” 

is.null(vector_name) - Checks if the entire vector is empty 

length(vector_name) - Number of elements present inside the vector

Syntax:

~~~
> x <- c(1,2,3,4)
> class (x)
[1] "numeric"
> str (x)
num [1:4] 1 2 3 4 
> length (x)
[1] 4

~~~
{: .language-r}

[FIXME add code image]

####  **Subsetting a vector**

R uses one-indexing mechanism where the elements in the vector start with an index number of one.

vector_name[4] - Element at the fourth position (index) in the vector

vector_name[1:4] - Elements from positions 1 to 4 in the vector

vector_name[c(1,4)] - Elements at positions 1 & 4 only in the vector

vector_name[-c(1,4)] - All elements except those at positions 1 & 4 in the vector

[FIXME add code image]

#### **Sorting a vector**

Sorting of a vector can be performed using two different functions

sort(vector) - Sorts the vector numerically or alphabetically based on vector type 
              (ascending by default)

order(vector) - Returns the indices of the vector in the order they would appear when 
                the vector is sorted (ascending by default)
                
[FIXME add code image]


### **2. DATA FRAME** 

Data frames are used for storing Data tables in R. They are two-dimensional array structure and
are similar to tables where each column represents one variable. The main features to note about 
a data frame are: 

• Columns can be of different data types

• Each column name must be unique 

• Each column should be of same length i.e. contain the same number of elements

Data frames in R can be created in two ways: 

• Using data.frame() command 

• Importing data from files such as .csv, .xlsx etc.

**data.frame() FUNCTION:**

While using the command we can follow the below syntax 
    data.frame( column_1, column_2, column_3, …………………….) 
    
Make sure that the names of the columns are unique and are of same length.

                
        

{% include links.md %}