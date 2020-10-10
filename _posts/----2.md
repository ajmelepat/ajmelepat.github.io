---
layout: post
author: Harika Kanthi
title: Python basics to know for Data science interviews
date: 2020-10-10T04:31:23.164Z
thumbnail: /assets/img/posts/mobile-phone-1513945_640.jpg
category: Data Science
summary: Basics questions asked in interview on python
---


**What is python and why python?**



A programming language invented by Guido van Rossum which is used for high level programming.

It is a very popular language because it is free source and easy to learn.

The community for python is very big and has been growing.

Works on different platforms like Linux, Mac, etc.

Can be used for mathematics, web development, software development etc.

It is interpretable.

It has a lot of modules with pre-defined functions that are easy to access and use which work efficiently and effectively.





**Difference between lists and tuples?**

Lists are mutable objects that is they can be edited

Tuples are immutable that is they cannot be edited

Tuples are much faster than lists





**Local variables and global variables?**

Variables that can accessed within a function is called a local variable, whereas variables that can be accessed throughout the program is called global variable.

The variables that are declared outside a function that is in the global environment are called global variable.

The variables created inside a function is called a local variable. These variables are not present in the global space.

When the variable inside the function is searched, it searches the local environment, if not found it searches the global environment.





**Is python case sensitive?**

Yes, python is case sensitive as in python "go" is different from "Go"





**Is indentation required in python?**

Yes, indentation plays a very important part of python.

Any code within loops or functions etc. need indentations to be specified

Usual indentation is a space of 4.







**Difference between arrays and lists?**

Arrays are elements which can hold only single data type elements while lists can have multiple data types.

Arrays helps perform vector operations while lists does not allow.





**What is a lambda function?**

A lambda function is an anonymous function created which can hold any number of parameters but always have only one expression to execute. They usually are small functions .





**Difference between For loop and While loop?**

While loops are the loops which usually take a condition and execute the expressions given the condition is True and

It also requires initialisation and increment

For loops are the loops which usually iterate over an object that can be iterated.





**Purpose of is, not and in ?**

"Is" is an operation which returns True when the variables are equal and False if not

"In" is an operation which checks for a variable in another object and returns True if present and False if not

"Not" returns the opposite of the Boolean value





**What is a tuple?**

A tuple is a collection of elements/components which can be of different or the same data types.

The tuples are immutable objects that is they cannot be changed once created.

e.g. storing usernames, date of birth, name, things that cause a huge change can be put in a tuple etc.





**What is a list?**

A data structure in python which is a collection of same or different data types.

The lists are mutable objects which gives us the flexibility to change it even after creating it.

We prefer them over lists due to this mutable nature.





**Can we have repeated values?**

We can have repeated values in tuples and lists but not in case of dictionaries and sets.





**What is a dictionary ?**

A dictionary is a collection of key : value pairs which are separated by a colon.

Each key has its corresponding values.

It is mutable.

Dictionaries' keys are its indexes



**What is an index?**

Indexes are used to locate a certain value in a given set of data.

Indexes are the identifiers of the rows.

In python it starts from 0 to the length of the object.





**What are negative indexes?**

Negative indexes are similar to positive indexes in python.

They are used to select in a reverse order.

Negative indexes start with -1 for the last value, -3 for the second last in the object and so on.





**Advantages of arrays over lists?**

Arrays are vectorised and help in element wise operations unlike lists which do not support it.

Numpy is a more efficient and convenient where we can do all vector and matrix operations.

Arrays are faster than lists



**Difference between delete, remove, pop?**

**or**

**How to remove elements in a list?**

Pop is a function that removes the last element or the element whose index is specified and prints it to the console.

Remove is a function that removes the element given from the list

Delete is a function that deletes the element from the list based on the index given.





**Difference between module and package?**

Module is the single file while package is a collection of modules

For instance scipy is a package whereas stats is a module.





**Difference between iterator, iterable, iteration?**

Iterable is the object that we can iterate over.

Iterator is the state during the iteration. It is the object which is used to iterate over an iterable.

Iteration is defined as the act or process of repeating. Iteration is the process of iterating over a variable.





**Difference in Dict and list comprehensions ?**

They are method that are similar to writing a comprehension which helps us store them.They are similar to creating them traditionally\[Expression if statements for loop if statements]

Dict comprehension : { key: value loop}

e.g. {x: x\*\*2 for x in list}

List comprehension : \[expr loop]

e.g. \[x\*\*2 for x In list]





Libraries you used?

Numpy

Pandas

Matplotlib

Seaborn

Scikit

Sklearn

Scipy





**Why anaconda?**

Anaconda is usually popular due as it tries to bring together many different data science tools.

It works faster and efficiently

It is user friendly.







**Python IDEs?**

IDE - integrated development environment

Jupyter Notebook, PyCharm, and Spyder are all good Python IDEs, but Jupyter Notebook is arguably the best for data science.





**What errors did you face?**

* Indentation error: When we do not give the right indentations usually while writing loops we face this error
* Key error: When the key is not present in the object, this error is returned
* Syntax error: When the proper structure is not defined while writing a syntax, we get this error
* File Not Found Error: When we load a file while does not exist in the same folder or in the defined folder we get this error
* Keyboard Interrupt error: When the user explicitly stops the execution of the code we get this error
* Name error: When we specify an object which is undefined that is not found in local or global environments we get this error
* Type error: When we apply a function to an incorrect data type we get this kind of error

e.g. int("dog")

* Value error: When we apply a function to an argument to correct type but improper value
* Attribute error: Using functions that do not work on the object given we get these error

e.g. emptylist.append(a)





**What is a variable?**

The variable is a temporary storage for the values.

We can access those values by calling them.

We can overwrite those values.





**What is the difference between set and dictionaries?**

Dictionaries have key value pairs while sets take the values and removes duplicates and gives values

Dictionaries are indexed where index is the key while sets are unindexed and unordered.

**Use of functions?**

The use of creating functions in python is easy accessibility of code.

That is where we want a code to not be written each time.





**Map, reduce, filter, accumulate?**

* The map function has two arguments function and an iterable. It maps the function to each value in the iterable.

Map(lambda x:x+1, list)

* Filter is also a function that takes two arguments function and an iterables. It filters the elements in the iterable based on the function given.

Filter(lambda x:x<10,list)

* Reduce is a function that performs computation on a list and returns one single value.

Reduce(lambda x,y: x+y, list)

* Accumulate is a function that performs computation on a list and returns values at each step during the function

Accumulate( list,lambda x,y:x+y)

To access all these we need to store them.