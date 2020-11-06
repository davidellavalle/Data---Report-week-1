insert table of contents

# Data - Report week 1

A computer program is a sequence of instructions that specifies how to perform a computation.
* **input** - Get data from the keyboard, a file, or some other device.
* **output** - Display data on the screen or send data to a file or other device.
* **assignment** - Set the value of a storage location denoted by a variable name.
* **math and logic** - Perform basic mathematical operations like addition, and multiplication, and logical operations like and, or, and not.
* **conditional execution** - Check for certain conditions and execute the appropriate sequence of statements.
* **repetition** - Perform some action repeatedly, usually with some variation.
* **Debugging** – removing Bugs -  Three kinds of errors can occur in a program: syntax errors, runtime errors, and semantic errors.

## **Data types**

### **Numeric**

#### **Integer**

1 2 3 4 -1 -2 -3 -4…..  
This value is represented by **int class**. It contains positive or negative whole numbers (without fraction or decimal). In Python there is no limit to how long an interger value can be.

#### **Float**

1,3  1,4  1,6  5,4   6,4   -3,4  -4,3   
This value is represented by **float class**. It is a real number with floating point representation. It is specified by a decimal point. Optionally, the character e or E followed by a positive or negative integer may be appended to specify scientific notation.

### **Boolean**

This is a value that expresses a truth value (which can be **either true or false**) 

### **Sequential**

#### **List**

A list is created by placing all the items (elements) inside a square bracket [ ], separated by commas. It doesn't need to be homogeneous but can contain Integers, Strings or Objects at the time. List are mutable and can be changed after their creation.  
The elements in a list are Indexed and **0 is the first index** -> this means that the last element will be n-1 (eg. 25 elements in the list, index 0:24) 

**Some of the most common Lists methods:**
* append() - Add an element to the end of the list
* extend() - Add all elements of a list to the another list
* insert() - Insert an item at the defined index
* remove() - Removes an item from the list
* pop() - Removes and returns an element at the given index
* clear() - Removes all items from the list
* index() - Returns the index of the first matched item
* count() - Returns the count of number of items passed as an argument
* sort() - Sort items in a list in ascending order
* reverse() - Reverse the order of items in the list
* copy() - Returns a shallow copy of the list

```python
>>> mylist = []
>>> mylist.append('this')
>>> mylist
['this']
>>> mylist.insert(1, 'thing')
>>> mylist
['this', 'thing']
>>> mylist.remove('thing')
>>> mylist
['this']
```

#### **Tuple**
A Tuple is created by placing all the items (elements) inside a round bracket ( ). It is unchangeable. In Dictionary we can create keys using tuples  
Indexes works as per LIST: with positive and negative indexes [1] [2] [-1] [-2]  or with range of indexes [2:5] [-3:-1]
```python
thistuple = ("apple", "banana", "cherry", "orange", "kiwi", "melon", "mango")
print(thistuple[-4:-1])
('orange', 'kiwi', 'melon')
```
To the unchangeability of the tuple there is a workaround: you can convert the tuple into a list, change the list, and convert the list back into a tuple.
```python
y = list(x)
y[1] = "kiwi"
x = tuple(y)
print(x)
("apple", "kiwi", "cherry")
```

#### **String**

A string is a collection of one or more characters put in a single quote, double-quote (Double quotes can contain singles) or triple quote (can even span multiple lines)
```python
"Ben's bike is broken!"
>>> message = """This message will
... span several
... lines."""
```

**Some of the most common string methods:**
* s.lower(), s.upper() — returns the lowercase or uppercase version of the string   
* s.isalpha()/s.isdigit()/s.isspace()… — tests if all the string chars are in the various character classes  
* s.startswith(‘ai’), s.endswith(‘ai’) — tests if the string starts or ends with the given ai strin  
* s.find(‘other’) — searches for the given other string (not a regular expression) within s, and returns the first index where it begins or -1 if not found  
* s.replace(‘old’, ‘new’) — returns a string where all occurrences of ‘old’ have been replaced by ‘new’ 

### **Container**

#### **Set**

Set is an unordered collection of data type that is iterable, mutable and has no duplicate elements (Uniques).  
The major advantage of using a set, as opposed to a list, is that it has a highly optimized method for checking whether a specific element is contained in the set.
```python
Set()
set1 = set("CodeDataAI")  
print(set1)
	{'o', 'D', 'a', 'A', 'e', 't', 'I', 'd', 'C'}

set1 = set(["Code", "Data", "Code"])  
print(set1)
	{'Data', 'Code'}
```
Adding and removing elements to a Set - 
* set.add
* set.update
* set.remove
* discard

#### **Dictionary**

##### How to understand the data Type?

```python
>>> type("Hello, World!")
<class 'str'>
>>> type(17)
<class 'int'>
```

##### How to print your result

```python
print("Hello, World!")
```
Escape sequence can be used to modify the format  

\\	Backslash (\)
\'	Single quote (')
\"	Double quote (")
\b	Backspace
\n	Linefeed
\t	Tab

= vs ==
