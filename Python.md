# Python Interview Questions and Answers

## Python Interview Questions for Freshers

### ****1. What is Python? List some popular applications of Python in the world of technology.****

Python is a widely-used general-purpose, high-level programming language. It was created by Guido van Rossum in 1991 and further developed by the Python Software Foundation. Python is known for its simple, readable syntax and allows programmers to express their concepts in fewer lines of code.\
It is used for:

* Data science & machine learning (with libraries like Pandas, NumPy, and TensorFlow)
* Web development (using frameworks like Django and Flask)
* Automation & scripting
* Artificial Intelligence & Deep Learning
* Data analysis & visualization
* Game development
* Software development

### ****2. What are the benefits of using Python language as a tool in the present scenario?****

The following are the benefits of using Python language:

* Object-Oriented Language
* High-Level Language
* Dynamically Typed language
* Extensive support for Machine Learning Libraries
* Presence of third-party modules
* Open source and community development
* Portable and Interactive
* Cross-Platform

### ****3. Is Python a compiled language or an interpreted language?****

Most of us may be surprised to know that python is actually both a compiled and interpreted language., when Python code is executed, it is first compiled into bytecode and then bytecode is interpreted by the Python Virtual Machine (PVM) on the underlying platform (machine + operating system). This hybrid approach allows python to balance ease of development with execution efficiency.

### 4. What is a dynamically typed language?

[Typed languages](https://www.geeksforgeeks.org/what-is-a-typed-language/) are the languages in which we define the type of data type and it will be known by the machine at the compile-time or at runtime. Typed languages can be classified into two categories:

* ****Statically typed languages: ****In this type of language, the data type of a variable is known at the compile time which means the programmer has to specify the data type of a variable at the time of its declaration. 
* ****Dynamically typed languages: ****These are the languages that do not require any pre-defined data type for any variable as it is interpreted at runtime by the machine itself. In these languages, interpreters assign the data type to a variable at runtime depending on its value.

### ****5. What does the ‘#’ symbol do in Python?****

‘#’ is used to comment on everything that comes after on the line.

### ****6. What is the difference between a Mutable datatype and an Immutable data type?****

* Mutable data types can be edited i.e., they can change at runtime. Eg – List, Dictionary, etc.
* Immutable data types can not be edited i.e., they can not change at runtime. Eg – String, Tuple, etc.

### ****7. How are arguments passed by value or by reference in Python?****

In Python, arguments are passed by object reference (also called “pass by assignment”). This means that functions receive references to the same objects:

* Mutable objects (like lists or dictionaries) can be modified within the function.
* Immutable objects (like integers or strings) cannot be changed and reassigning them inside the function doesn’t affect the original object.

### ****8. What is the difference between a Set and Dictionary?****
<span style="color:red">Python 3.7以后Dict都是有序的,之前都是无序的</span>
字典有序,map格式
集合无序,无格式
The set is unordered collection of unique items that is iterable and mutable. A dictionary in Python is an ordered collection of data values, used to store data values like a map.

### ****9. What is List Comprehension? Give an Example.****

List comprehension is a syntax construction to ease the creation of a list based on existing iterable.

For Example:

Python`li = [i for i in range(1, 10)]
`

### ****10. How is a dictionary different from a list?****
1. 访问方面index, key
2. 一个有序一个无序(dict 3.5之前无序)
3. sequential data/associative data
A list is an ordered collection of items accessed by their index, while a dictionary is an unordered collection of key-value pairs accessed using unique keys. Lists are ideal for sequential data, whereas dictionaries are better for associative data. For example, a list can store \[10, 20, 30], whereas a dictionary can store {“a”: 10, “b”: 20, “c”: 30}.

### ****11. What is a pass in Python?****

Pass means performing no operation or in other words, it is a placeholder in the compound statement, where there should be a blank left and nothing has to be written there.

### ****12. What is the difference between / and // in Python?****

/ represents precise division (result is a floating point number) whereas // represents floor division (result is an integer). For Example:

> 5//2 = 2
>
> 5/2 = 2.5

### ****13. How is Exceptional handling done in Python?****

There are 3 main keywords i.e. try, except, and finally which are used to catch exceptions and handle the recovering mechanism accordingly. Try is the block of a code that is monitored for errors. Except block gets executed when an error occurs.

The beauty of the final block is to execute the code after trying for an error. This block gets executed irrespective of whether an error occurred or not. Finally, block is used to do the required cleanup activities of objects/variables.

### ****14. What is a lambda function?****

A lambda function is an anonymous function. This function can have any number of parameters but, can have just one statement. For Example:

Python`a = lambda x, y : x*y
print(a(7, 19))
`

### ****15. Difference between for loop and while loop in Python****

The “for” Loop is generally used to iterate through the elements of various collection types such as [List](https://www.geeksforgeeks.org/python-lists/), [Tuple](https://www.geeksforgeeks.org/python-tuples/), [Set](https://www.geeksforgeeks.org/sets-in-python/), and [Dictionary](https://www.geeksforgeeks.org/python-dictionary/). Developers use a “for” loop where they have both the conditions **start and the end**. Whereas, the “while” loop is the actual looping feature that is used in any other programming language. Programmers use a Python while loop where they just have the **end conditions**.

### 16. Can we Pass a function as an argument in Python?

Yes, Several arguments can be passed to a function, including objects, variables (of the same or distinct data types), and functions. Functions can be passed as parameters to other functions because they are objects. Higher-order functions are functions that can take other functions as arguments.

To read more, refer to the article: [Passing function as an argument in Python](https://www.geeksforgeeks.org/passing-function-as-an-argument-in-python/)

### 17. What are \*args and \*\*kwargs?

To pass a variable number of arguments to a function in Python, use the special syntax [\*args and \*\*kwargs](https://www.geeksforgeeks.org/args-kwargs-python/) in the function specification. Both are to send a variable-length argument list. The syntax \*args is used to pass a non-keyworded, variable-length argument list.

*args allows a function to accept any number of positional arguments as a **tuple**.可变长参数以元组形式传入.
**kwargs allows a function to accept any number of keyword arguments as a dictionary.可变长参数以字典形式传入.

### 18. Is Indentation Required in Python?

Yes, [indentation](https://www.geeksforgeeks.org/indentation-in-python/) is required in Python. A [Python](https://www.geeksforgeeks.org/python-programming-language/) interpreter can be informed that a group of statements belongs to a specific block of code by using Python indentation. Indentations make the code easy to read for developers in all programming languages but in Python, it is very important to indent the code in a specific order.

### 19. What is a Variable Scope in Python?

The location where we can find a variable and also access it if required is called the scope of a variable.

* ****Python Local variable:**** Local variables are those that are initialized within a function and are unique to that function. It cannot be accessed outside of the function.
* ****Python Global variables:**** Global variables are the ones that are defined and declared outside any function and are not specified to any function.
* ****Module-level scope:**** It refers to the global objects of the current module accessible in the program.
* ****Outermost scope: ****It refers to any built-in names that the program can call. The name referenced is located last among the objects in this scope.

### 20. What is docstring in Python?

Python documentation strings (or docstrings) provide a convenient way of associating documentation with Python modules, functions, classes, and methods.

* ****Declaring Docstrings:**** The docstrings are declared using ”’triple single quotes”’ or “””triple double quotes””” just below the class, method, or function declaration. All functions should have a docstring.
* ****Accessing Docstrings:**** The docstrings can be accessed using the \_\_doc\_\_ method of the object or using the help function.

### 21. What is a break, continue, and pass in Python? 

* [break statement](https://www.geeksforgeeks.org/python-break-statement/) is used to terminate the loop or statement in which it is present. After that, the control will pass to the statements that are present after the break statement, if available.
* [Continue](https://www.geeksforgeeks.org/python-continue-statement/) is also a loop control statement just like the break statement. continue statement is opposite to that of the break statement, instead of terminating the loop, it forces to execute the next iteration of the loop.
* [Pass ](https://www.geeksforgeeks.org/python-pass-statement/)means performing no operation or in other words, it is a placeholder in the compound statement, where there should be a blank left and nothing has to be written there.

### 22. What are Built-in data types in Python?

The following are the standard or built-in data types in Python:
整型--int

布尔型--bool

字符串--str

列表--list

元组--tuple

字典--dict
* ****Numeric: ****The numeric data type in Python represents the data that has a numeric value. A numeric value can be an integer, a floating number, a Boolean****, ****or even a complex number.

* ****Sequence Type: T****he sequence Data Type in Python is the ordered collection of similar or different data types. There are several sequence types in Python:

  * [Python String](https://www.geeksforgeeks.org/python-string/)
  * [Python List](https://www.geeksforgeeks.org/python-lists/)
  * [Python Tuple](https://www.geeksforgeeks.org/python-tuples/)
  * [Python range](https://www.geeksforgeeks.org/python-range-function/)

* ****Mapping Types: ****In Python, hashable data can be mapped to random objects using a mapping object. There is currently only one common mapping type, the dictionary, and mapping objects are mutable.
  * [Python Dictionary](https://www.geeksforgeeks.org/python-dictionary/)

* ****Set Types: ****In Python, a [Set](https://www.geeksforgeeks.org/sets-in-python/) is an unordered collection of data types that is iterable, mutable, and has no duplicate elements. The order of elements in a set is undefined though it may consist of various elements.

### 23. How do you floor a number in Python?

The Python math module includes a method that can be used to calculate the floor of a number. 

* [floor() ](https://www.geeksforgeeks.org/floor-ceil-function-python/)method in Python returns the floor of x i.e., the largest integer not greater than x. 
* Also, The method ceil(x) in Python returns a ceiling value of x i.e., the smallest integer greater than or equal to x.

## Intermediate Python Interview Questions

### ****24. What is the difference between xrange and range functions?****

range() and xrange() are two functions that could be used to iterate a certain number of times in for loops in Python. 

* In Python 3, there is no xrange, but the range function behaves like xrange.

* In Python 2

  * ****range() ****– This returns a **range** object, which is an immutable sequence type that generates the numbers on demand. 
  * ****xrange()**** – This function returns the **generator** object that can be used to display numbers only by looping. The only particular range is displayed on demand and hence called lazy evaluation.
python2和python3的range（100）的区别
range(100) 返回列表, Python 3: range(100) 返回可迭代对象

### ****25. What is Dictionary Comprehension? Give an Example****

Dictionary Comprehension is a syntax construction to ease the creation of a dictionary based on the existing iterable.

For Example: **my\_dict = {i:i+7 for i in range(1, 10)}**

### ****26. Is Tuple Comprehension? If yes, how, and if not why?****

> (i for i in (1, 2, 3))

Tuple comprehension is not possible in Python because it will end up in a generator, not a tuple comprehension.

### ****27. Differentiate between List and Tuple?****

Let’s analyze the differences between List and Tuple:

****List****

* Lists are Mutable datatype.
* Lists consume more memory
* The list is better for performing operations, such as insertion and deletion.
* The implication of iterations is Time-consuming

****Tuple****

* Tuples are Immutable datatype.
* Tuple consumes less memory as compared to the list
* A Tuple data type is appropriate for accessing the elements
* The implication of iterations is comparatively Faster

### ****28. What is the difference between a shallow copy and a deep copy?****
浅拷贝 不递归, 只拷贝引用
深拷贝 递归拷贝全部,创建一个新的.
A shallow copy creates a new object but does not recursively copy nested objects. Instead, it copies references to the original objects.
A deep copy recursively copies all nested objects, creating completely independent objects.

### ****29. Which sorting technique is used by sort() and sorted() functions of python?****

Python uses the [*****Tim Sort*****](https://www.geeksforgeeks.org/timsort/) algorithm for sorting. It’s a stable sorting whose worst case is O(N log N). It’s a hybrid sorting algorithm, derived from merge sort and insertion sort, designed to perform well on many kinds of real-world data.
sorted() VS sort()
list.sort() 在list基础上修改,无返回值
sorted有返回值是新的list

### ****30. What are Decorators?****

[Decorators](https://www.geeksforgeeks.org/decorators-in-python/) are a very powerful and useful tool in Python as they are the specific change that we make in Python syntax to alter functions easily.

### ****31. How do you debug a Python program?****

By using this command we can debug a Python program:

> python -m pdb python-script.py

### ****32. What are Iterators in Python?****

In Python, iterators are used to iterate a group of elements, containers like a list. Iterators are collections of items, and they can be a list, tuples, or a dictionary. Python iterator implements \_\_itr\_\_ and the next() method to iterate the stored elements. We generally use loops to iterate over the collections (list, tuple) in Python.

### ****33. What are Generators in Python?****

In Python, the [generator ](https://www.geeksforgeeks.org/generators-in-python/)is a way that specifies how to implement iterators. It is a normal function except that it yields expression in the function. It does not implement \_\_itr\_\_ and \_\_next\_\_ method and reduces other overheads as well.

If a function contains at least a yield statement, it becomes a generator. The yield keyword pauses the current execution by saving its states and then resumes from the same when required.

### ****34. Does Python supports multiple Inheritance?****

Python does support multiple [inheritances](https://www.geeksforgeeks.org/inheritance-in-python/), unlike Java. Multiple inheritances mean that a class can be derived from more than one parent class.

### ****35. What is Polymorphism in Python?****



### ****36. Define encapsulation in Python?****

It refers to the bundling of data (variables) and methods (functions) into a single unit (class) and restricting direct access to some components of the object to protect the integrity of the data.(Prevents direct access to class variables from outside the class.)

### ****37. How do you do data abstraction in Python?****

[Data Abstraction](https://www.geeksforgeeks.org/data-abstraction-in-python/) is providing only the required details and hides the implementation from the world. It can be achieved in Python by using interfaces and abstract classes.

### ****38. How is memory management done in Python?****
堆内存
垃圾回收器
Python uses its private **heap space** to manage the memory. Basically, all the objects and data structures are stored in the private heap space. Even the programmer can not access this private space as the interpreter takes care of this space. Python also has an inbuilt **garbage collector**, which recycles all the unused memory and frees the memory and makes it available to the heap space.

### ****39. How to delete a file using Python?****

We can delete a file using Python by following approaches:

* os.remove()
* os.unlink()

### 40. What is slicing in Python?

[Python Slicing](https://www.geeksforgeeks.org/python-slice-function/) is a string operation for extracting a part of the string, or some part of a list. With this operator, one can specify where to start the slicing, where to end, and specify the step. List slicing returns a new list from the existing list.

> Syntax: Lst\[ Initial : End : IndexJump ]

### ****41. What is a namespace in Python?****

A namespace is a naming system used to make sure that names are unique to avoid naming conflicts.

![Python-Interview-Questions](https://media.geeksforgeeks.org/wp-content/uploads/20250131173151505983/Python-Interview-Questions.webp)

## Advanced Python Interview Questions & Answers 

### ****42. What is PIP?****

PIP is an acronym for Python Installer Package which provides a seamless interface to install various Python modules. It is a command-line tool that can search for packages over the internet and install them without any user interaction.

### ****43. What is a zip function?****

Python [zip() function](https://www.geeksforgeeks.org/zip-in-python/) returns a zip object, which maps a similar index of multiple containers. It takes an iterable, converts it into an iterator and aggregates the elements based on iterables passed. It returns an iterator of **tuples**(tuple list).

### ****44. What are Pickling and Unpickling?****
pickling 将python对象serialization成byte stream
Unpickling 将byte stream转换成python object
Pickle module accepts any Python object and converts it into a string representation and dumps it into a file by using the dump function, this process is called pickling. While the process of retrieving original Python objects from the stored string representation is called unpickling.

### ****45****. What is the difference between `@classmethod`, `@staticmethod`, and instance methods in Python?

1\. Instance Method operates on an instance of the class and has access to instance attributes and takes self as the first parameter. Example:

> def method(self):

2\. Class Method directly operates on the class itself and not on instance, it takes cls as the first parameter. and defined with[ @classmethod.](https://www.geeksforgeeks.org/classmethod-in-python/)

> ****Example: ****@classmethod def method(cls):

3\. Static Method does not operate on an instance or the class and takes no self or cls as an argument and is defined with [@staticmethod.](https://www.geeksforgeeks.org/python-staticmethod/)

> ****Example: ****@staticmethod def method(): align it and dont bolod anything and not bullet points

### ****46. ****What is `__init__()` in Python and how does `self` play a role in it?

[\_\_init\_\_() method](https://www.geeksforgeeks.org/__init__-in-python/) in Python is equivalent to constructors in OOP terminology. It is a reserved method in Python classes and is called automatically whenever a new object is instantiated. This method is used to **initialize the object’s attributes** with values. While \_\_init\_\_() initializes the object, it does not allocate memory. Memory allocation for a new object is handled by the \_\_new\_\_() method, which is called before \_\_init\_\_(). The `self` parameter in `__init__()` refers to **the instance of the class** being created as it allows access to the instance’s attributes and methods. *`self`* must be explicitly declared as the first parameter in all instance methods, including `__init__()`.

Python`class MyClass:
    def __init__(self, value):
        self.value = value  # Initialize object attribute

    def display(self):
        print(f"Value: {self.value}")

obj = MyClass(10)
obj.display() 
`

### ****47. Write a code to display the current time?****

Python`import time

currenttime= time.localtime(time.time())
print ("Current time is", currenttime)
`

### 48. What are Access Specifiers in Python?

Python uses the ‘\_’ symbol to determine the access control for a specific data member or a member function of a class. A Class in Python has three types of [Python access modifiers](https://www.geeksforgeeks.org/access-modifiers-in-python-public-private-and-protected/):

* ****Public Access Modifier:**** The members of a class that are declared public are easily accessible from any part of the program. All data members and member functions of a class are public by default. 
* ****Protected Access Modifier****:The members of a class that are declared protected are only accessible to a class derived from it. All data members of a class are declared protected by adding a single underscore ‘\_’ symbol before the data members of that class. 
* ****Private Access Modifier****:The members of a class that are declared private are accessible within the class only, the private access modifier is the most secure access modifier. Data members of a class are declared private by adding a double underscore ‘\_\_’ symbol before the data member of that class. 

### 49. What are unit tests in Python?

Unit Testing is the first level of software testing where the smallest testable parts of the software are tested. This is used to validate that each unit of the software performs as designed. The unit test framework is Python’s xUnit style framework. The White Box Testing method is used for Unit testing.

### 50. Python Global Interpreter Lock (GIL)?

[Python Global Interpreter Lock](https://www.geeksforgeeks.org/what-is-the-python-global-interpreter-lock-gil/) (GIL) is a type of process lock that is used by Python whenever it deals with processes. Generally, Python only uses only one thread to execute the set of written statements. The performance of the single-threaded process and the multi-threaded process will be the same in Python and this is because of GIL in Python. We can not achieve multithreading in Python because we have a global interpreter lock that restricts the threads and works as a single thread.

### 51. What are Function Annotations in Python?

[Function Annotation](https://www.geeksforgeeks.org/function-annotations-python/) is a feature that allows you to add metadata to function parameters and return values. This way you can specify the input type of the function parameters and the return type of the value the function returns.

Function annotations are arbitrary Python expressions that are associated with various parts of functions. These expressions are evaluated at compile time and have no life in Python’s runtime environment. Python does not attach any meaning to these annotations. They take life when interpreted by third-party libraries, for example, mypy.

### 52. What are Exception Groups in Python?

The latest feature of Python 3.11, [Exception Groups](https://www.geeksforgeeks.org/exception-groups-in-python/). The ExceptionGroup can be handled using a new except\* syntax. The \* symbol indicates that multiple exceptions can be handled by each except\* clause.

ExceptionGroup is a collection/group of different kinds of Exception. Without creating Multiple Exceptions we can group together different Exceptions which we can later fetch one by one whenever necessary, the order in which the Exceptions are stored in the Exception Group doesn’t matter while calling them.

```
try:
raise ExceptionGroup('Example ExceptionGroup', (
TypeError('Example TypeError'),
ValueError('Example ValueError'),
KeyError('Example KeyError'),
AttributeError('Example AttributeError')
))
except* TypeError:
...
except* ValueError as e:
...
except* (KeyError, AttributeError) as e:
...
```

### ****53. What is Python Switch Statement?****

From version 3.10 upward, Python has implemented a switch case feature called “structural pattern matching”. You can implement this feature with the match and case keywords. Note that the underscore symbol is what you use to define a default case for the switch statement in Python.

****Note****: Before Python 3.10 Python doesn’t support match Statements.

Python`match term:
   case pattern-1:
   action-1
   case pattern-2:
   action-2
   case pattern-3:
   action-3
   case _:
   action-default
`

### 54. What is Walrus Operator?

Walrus Operator allows you to assign a value to a variable within an expression. This can be useful when you need to use a value multiple times in a loop, but don’t want to repeat the calculation.

Walrus Operator is represented by the \`:=\` syntax and can be used in a variety of contexts including while loops and if statements.

****Note: ****Python versions before 3.8 doesn’t support Walrus Operator.

Python`names = ["Jacob", "Joe", "Jim"]

if (name := input("Enter a name: ")) in names:
    print(f"Hello, {name}!")
else:
    print("Name not found.")
`\

### 55. os.path.join() V.S. str.join()
os.path.join() 是 os.path 模块中的一个方法，专门用于跨平台地拼接文件路径
str.join(iterable) 是字符串的方法，专门用于将多个字符串连接成一个字符串，通常用于处理 列表、元组等可迭代对象。

### 56. python中什么元素为假？
0，空字符串(empty string)，空列表(empty list)、空字典(empty dict)、空元组(empty tuple)、None, False

### 57. 请将[i for i in range(3)]改成生成器
列表表达式的【】改为（）即可变成生成器
函数在返回值得时候出现yield就变成生成器，而不是函数了；
(i for i in range(3))

### 58.python字典和json字符串相互转换方法?
json.dumps()字典转json字符串
json.loads()json字符串转字典