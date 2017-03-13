# Programming Principles
Follow these principles when programming.

## Version Control
Version control should be used for all projects, regardless of the size.

#### Continuous Integration
Currently using TravisCI for github integration.

#### Git
__github__
* github offers free repository hosting for all opensource coding projects
* A free github student account offers unlimited private repository hosting.

#### SVN
Another method of version control. Similar to git, but files are stored on a central repository, rather than distributed as with git repositories.

__tortoise svn__
* good option for svn

## Object Oriented Programming (OOP)
__References__
* [Object Oritented Design Standards](http://www.literateprogramming.com/oostnd.pdf)
___
Taken from [stackoverflow post](http://stackoverflow.com/questions/399656/are-there-any-rules-for-oop)

Summarized from Agile Software Development Principles, Patterns, and Practices. These principles are the hard-won product of decades of experience in software engineering. They are not the product of a single mind, but they represent the integration and writings of a large number of software developers and researchers. Although they are presented here as principles of object-oriented design, they are really special cases of long-standing principles of software engineering.

__SRP The Single Responsibility Principle__ A class should have only one reason to change.

__OCP The Open-Closed Principle Software__ entities (classes, packages, methods, etc.) should be open for extension, but closed for modification.

__LSP The Liskov Substition__ Principle Subtypes must be substitutable for their base types.

__DIP The Dependency Inversion Principle__ Abstractions should not depend upon details. Details should depend upons abstractions.

__ISP The Interface Segregation Principle__ Clients shold not be forced to depend upon methods that they do not use. Interfaces belong to clients, not to hierarchies.

__REP The Release-Reuse Equivalency__ Principle The granule of reuse is the granule of release.

__CCP The Common Closure Principle__ The classes in a package should be closed together against the same kinds of changes. A change that affects a closed package affects all the classes in that package and no other packages.

__CRP The Common Reuse Principle__ The classes in a package are reused together. If you reuse one of the classes in a package, you reuse them all.

__ADP The Acylcic Dependencies Principle__ Allow no cycles in the dependency graph.

__SDP The Stable Dependencies Principle__ Depend in the direction of stability.

__SAP The Stable Abstractions Principle__ A package should be as abstract as it is stable.
___
## Languages
### Python 3
[Python 3 Documentation](https://docs.python.org/3/)

#### Always Do:
* Include <code>#!/usr/bin/env python</code> at the top of every python file. This guarantees that the first python installation in the <code>$PATH</code> variable is used to execute the file. Read more on this [stackoverflow article](http://stackoverflow.com/questions/2429511/why-do-people-write-usr-bin-env-python-on-the-first-line-of-a-python-script).

#### Numpy
[Numpy Documentation](https://docs.scipy.org/doc/numpy/)

#### Scipy
[Scipy Documentation](https://docs.scipy.org/doc/scipy/reference/)


#### Matplotlib
__General Plotting__
* <code>import matpolotlib.pyplot as plt</code>

#### Openpyxl
Openpyxl is used to read and write excel sheets.

#### Cython
[Cython Documentation](http://cython.org/)

__General Info:__

Cython is an optimising static compiler for both the Python programming language and the extended Cython programming language (based on Pyrex). It makes writing C extensions for Python as easy as Python itself.

__Cython gives you the combined power of Python and C to let you__
* write Python code that calls back and forth from and to C or C++ code natively at any point.
* easily tune readable Python code into plain C performance by adding static type declarations.
* use combined source code level debugging to find bugs in your Python, Cython and C code.
* interact efficiently with large data sets, e.g. using multi-dimensional NumPy arrays.
* quickly build your applications within the large, mature and widely used CPython ecosystem.
* integrate natively with existing code and data from legacy, low-level or high-performance libraries and applications.

### C++
[Official C++ Documentation](https://isocpp.org/std/the-standard)


### Matlab

## Machine Learning
* [Principles of Machine Learning](https://www.edx.org/course/principles-machine-learning-microsoft-dat203-2x-2)

### Tensorflow
[TensorFlow Programmers Guide](https://www.tensorflow.org/programmers_guide/reading_data)
