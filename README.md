 {#keywords-and-identifiers}

    {\color{incolor}In [{\color{incolor}6}]:} \PY{k+kn}{import} \PY{n+nn}{keyword}
            
            \PY{n+nb}{print}\PY{p}{(}\PY{n}{keyword}\PY{o}{.}\PY{n}{kwlist}\PY{p}{)}
            \PY{n+nb}{print}\PY{p}{(}\PY{n}{keyword}\PY{o}{.}\PY{n}{iskeyword}\PY{p}{(}\PY{l+s+s1}{\PYZsq{}}\PY{l+s+s1}{True}\PY{l+s+s1}{\PYZsq{}}\PY{p}{)}\PY{p}{)}
            \PY{n+nb}{print}\PY{p}{(}\PY{n+nb}{len}\PY{p}{(}\PY{n}{keyword}\PY{o}{.}\PY{n}{kwlist}\PY{p}{)}\PY{p}{)} \PY{c+c1}{\PYZsh{} keywords defined by the interpreter}

    True
    35

        

#### Identifiers:

    1) Identifiers can consist - a-z, A-Z, 0-9, _
    2) cannot start with number
    3) cannot use keywords as identifier

    {\color{incolor}In [{\color{incolor}7}]:} \PY{k}{global} \PY{o}{=} \PY{l+m+mi}{1}
            \PY{n}{a}\PY{o}{@} \PY{o}{=} \PY{l+m+mi}{2}


              File "<ipython-input-7-4e489388dec1>", line 1
            global = 1
                   \^{}
        SyntaxError: invalid syntax
        

        

 {#comments-indentation-statement}

1.  Single line comment - \#

2.  multi line comments - “”" or ”’

<!-- -->

    {\color{incolor}In [{\color{incolor}9}]:} \PY{l+s+sd}{\PYZdq{}\PYZdq{}\PYZdq{}}
            \PY{l+s+sd}{    multi}
            \PY{l+s+sd}{    line}
            \PY{l+s+sd}{    comment}
            \PY{l+s+sd}{\PYZdq{}\PYZdq{}\PYZdq{}}

    {\color{outcolor}Out[{\color{outcolor}9}]:} '\textbackslash{}n    multi\textbackslash{}n    line\textbackslash{}n    comment\textbackslash{}n'

**Doc string** *(Documentation string)* **:** String that occurs in the
first statement of a module, function, class or method definition \*used
as **doc**

    {\color{incolor}In [{\color{incolor}10}]:} \PY{k}{def} \PY{n+nf}{double}\PY{p}{(}\PY{n}{n}\PY{p}{)}\PY{p}{:}
                 \PY{l+s+sd}{\PYZdq{}\PYZdq{}\PYZdq{}}
             \PY{l+s+sd}{    function to double the number}
             \PY{l+s+sd}{    \PYZdq{}\PYZdq{}\PYZdq{}}
                 \PY{k}{return} \PY{l+m+mi}{2}\PY{o}{*}\PY{n}{n}\PY{p}{;}
             \PY{n+nb}{print}\PY{p}{(}\PY{n}{double}\PY{p}{(}\PY{l+m+mi}{11}\PY{p}{)}\PY{p}{)}
             \PY{n+nb}{print}\PY{p}{(}\PY{n}{double}\PY{o}{.}\PY{n+nv+vm}{\PYZus{}\PYZus{}doc\PYZus{}\PYZus{}}\PY{p}{)}

    22

        function to double the number
        

        

**Indentation:**

    1) Maintian consistency in indentation through out the block
    2) ';' can be used as terminator

**Python Statement**:

    1) instructions that a python interpreter can execute are called python statements

**MultiLine Statements:**

    1) ()
    2) \
    3) ; -> multiple line statements in single line

    {\color{incolor}In [{\color{incolor}21}]:} \PY{n+nb}{print}\PY{p}{(}\PY{n+nb}{range}\PY{p}{(}\PY{l+m+mi}{10}\PY{p}{)}\PY{p}{)}
             
             \PY{k}{for} \PY{n}{i} \PY{o+ow}{in} \PY{n+nb}{range}\PY{p}{(}\PY{l+m+mi}{10}\PY{p}{)}\PY{p}{:}
                 \PY{n+nb}{print}\PY{p}{(}\PY{n}{i}\PY{p}{)}
                 \PY{n}{i} \PY{o}{=} \PY{n}{i} \PY{o}{+} \PY{l+m+mi}{2}
             \PY{n+nb}{print}\PY{p}{(}\PY{n}{i}\PY{p}{)}

    range(0, 10)
    0
    1
    2
    3
    4
    5
    6
    7
    8
    9
    11

        

 {#var-datatypes}

    {\color{incolor}In [{\color{incolor}33}]:} \PY{n}{a} \PY{o}{=} \PY{l+m+mi}{10}
             \PY{n+nb}{print}\PY{p}{(}\PY{n+nb}{type}\PY{p}{(}\PY{n}{a}\PY{p}{)}\PY{p}{)}
             \PY{n}{b} \PY{o}{=} \PY{l+m+mf}{5.5}
             \PY{n+nb}{print}\PY{p}{(}\PY{n+nb}{type}\PY{p}{(}\PY{n}{b}\PY{p}{)}\PY{p}{)}
             \PY{n}{c} \PY{o}{=} \PY{l+s+s2}{\PYZdq{}}\PY{l+s+s2}{ML}\PY{l+s+s2}{\PYZdq{}}
             \PY{n+nb}{print}\PY{p}{(}\PY{n+nb}{type}\PY{p}{(}\PY{n}{c}\PY{p}{)}\PY{p}{)}
             
             \PY{c+c1}{\PYZsh{} Multiple assignments}
             
             \PY{n}{a}\PY{p}{,} \PY{n}{b}\PY{p}{,} \PY{n}{c} \PY{o}{=} \PY{l+m+mi}{10}\PY{p}{,} \PY{l+m+mf}{5.5}\PY{p}{,} \PY{l+s+s2}{\PYZdq{}}\PY{l+s+s2}{ML}\PY{l+s+s2}{\PYZdq{}}
             
             \PY{c+c1}{\PYZsh{} Storage Locations}
             
             \PY{n+nb}{print}\PY{p}{(}\PY{n+nb}{id}\PY{p}{(}\PY{n}{a}\PY{p}{)}\PY{p}{)}
             \PY{n}{a1} \PY{o}{=} \PY{l+m+mi}{10}
             \PY{n+nb}{print}\PY{p}{(}\PY{n+nb}{id}\PY{p}{(}\PY{n}{a1}\PY{p}{)}\PY{p}{)}
             \PY{n}{a1} \PY{o}{=} \PY{l+m+mi}{15}
             \PY{n+nb}{print}\PY{p}{(}\PY{n+nb}{id}\PY{p}{(}\PY{n}{a1}\PY{p}{)}\PY{p}{)}
             \PY{n+nb}{print}\PY{p}{(}\PY{n+nb}{id}\PY{p}{(}\PY{n}{a}\PY{p}{)}\PY{p}{)}
             
             \PY{n}{j}\PY{o}{=} \PY{l+m+mf}{10.0}
             \PY{n}{k} \PY{o}{=} \PY{n+nb}{float}\PY{p}{(}\PY{l+m+mi}{10}\PY{p}{)}
             \PY{n+nb}{print}\PY{p}{(}\PY{n+nb}{id}\PY{p}{(}\PY{n}{j}\PY{p}{)}\PY{p}{)}
             \PY{n+nb}{print}\PY{p}{(}\PY{n+nb}{id}\PY{p}{(}\PY{n}{k}\PY{p}{)}\PY{p}{)}

    <class 'int'>
    <class 'float'>
    <class 'str'>
    140710936309792
    140710936309792
    140710936309952
    140710936309792
    2655974007480
    2655974007384

        

 {#data-types}

1.  Everything is an object in python:

    1.  data types are classes

    2.  variables are instances of the classes

2.  All functions have inbuilt attribute doc - returns doc string

3.  sys(System specific parameters and functions) module has path
    attribute and other

4.  Objects here are subclassable(we can inherit them from class
    Foo(object):pass)

5.  In python, object definition is looser(some objects neither have
    attributes nor methods and not all objects are subclassable)

6.  Everything is an object means it can be assigned to avar or passed
    as an argument to a function

7.  looser - creating and using classes and objects are easy with
    immense flexibility provided by python

**Numbers:**

    1) integer : int class
    2) float   : float class
    3) complex : complex class

type() - to know which class variable

isinstance() - to check if it belongs to particular class

    {\color{incolor}In [{\color{incolor}36}]:} \PY{k}{class} \PY{n+nc}{Foo}\PY{p}{:} 
                 \PY{n}{a} \PY{o}{=} \PY{l+m+mi}{5}
             \PY{n}{fooInstance} \PY{o}{=} \PY{n}{Foo}\PY{p}{(}\PY{p}{)}
             
             \PY{n+nb}{print}\PY{p}{(}\PY{n+nb}{isinstance}\PY{p}{(}\PY{n}{fooInstance}\PY{p}{,} \PY{n}{Foo}\PY{p}{)}\PY{p}{)}
             \PY{n+nb}{print}\PY{p}{(}\PY{n+nb}{isinstance}\PY{p}{(}\PY{n}{fooInstance}\PY{p}{,} \PY{p}{(}\PY{n+nb}{list}\PY{p}{,} \PY{n+nb}{tuple}\PY{p}{)}\PY{p}{)}\PY{p}{)}
             \PY{n+nb}{print}\PY{p}{(}\PY{n+nb}{isinstance}\PY{p}{(}\PY{n}{fooInstance}\PY{p}{,} \PY{p}{(}\PY{n+nb}{list}\PY{p}{,} \PY{n+nb}{tuple}\PY{p}{,} \PY{n}{Foo}\PY{p}{)}\PY{p}{)}\PY{p}{)}

    True
    False
    True

        

    {\color{incolor}In [{\color{incolor}41}]:} \PY{n}{numbers} \PY{o}{=} \PY{p}{[}\PY{l+m+mi}{1}\PY{p}{,}\PY{l+m+mi}{2}\PY{p}{,}\PY{l+m+mi}{3}\PY{p}{]}
             \PY{n}{result} \PY{o}{=} \PY{n+nb}{isinstance}\PY{p}{(}\PY{n}{numbers}\PY{p}{,} \PY{n+nb}{list}\PY{p}{)}
             \PY{n+nb}{print}\PY{p}{(}\PY{n}{result}\PY{p}{)}
             \PY{n}{a} \PY{o}{=} \PY{l+m+mi}{1}\PY{o}{+}\PY{l+m+mi}{2}\PY{n}{j}
             \PY{n+nb}{print}\PY{p}{(}\PY{n+nb}{isinstance}\PY{p}{(}\PY{n}{a}\PY{p}{,} \PY{n+nb}{complex}\PY{p}{)}\PY{p}{)}

    True
    True

        

    {\color{incolor}In [{\color{incolor}40}]:} \PY{n}{help}\PY{p}{(}\PY{n+nb}{float}\PY{p}{)}

    Help on class float in module builtins:

    class float(object)
     |  float(x=0, /)
     |  
     |  Convert a string or number to a floating point number, if possible.
     |  
     |  Methods defined here:
     |  
     |  \_\_abs\_\_(self, /)
     |      abs(self)
     |  
     |  \_\_add\_\_(self, value, /)
     |      Return self+value.
     |  
     |  \_\_bool\_\_(self, /)
     |      self != 0
     |  
     |  \_\_divmod\_\_(self, value, /)
     |      Return divmod(self, value).
     |  
     |  \_\_eq\_\_(self, value, /)
     |      Return self==value.
     |  
     |  \_\_float\_\_(self, /)
     |      float(self)
     |  
     |  \_\_floordiv\_\_(self, value, /)
     |      Return self//value.
     |  
     |  \_\_format\_\_(self, format\_spec, /)
     |      Formats the float according to format\_spec.
     |  
     |  \_\_ge\_\_(self, value, /)
     |      Return self>=value.
     |  
     |  \_\_getattribute\_\_(self, name, /)
     |      Return getattr(self, name).
     |  
     |  \_\_getnewargs\_\_(self, /)
     |  
     |  \_\_gt\_\_(self, value, /)
     |      Return self>value.
     |  
     |  \_\_hash\_\_(self, /)
     |      Return hash(self).
     |  
     |  \_\_int\_\_(self, /)
     |      int(self)
     |  
     |  \_\_le\_\_(self, value, /)
     |      Return self<=value.
     |  
     |  \_\_lt\_\_(self, value, /)
     |      Return self<value.
     |  
     |  \_\_mod\_\_(self, value, /)
     |      Return self\%value.
     |  
     |  \_\_mul\_\_(self, value, /)
     |      Return self*value.
     |  
     |  \_\_ne\_\_(self, value, /)
     |      Return self!=value.
     |  
     |  \_\_neg\_\_(self, /)
     |      -self
     |  
     |  \_\_pos\_\_(self, /)
     |      +self
     |  
     |  \_\_pow\_\_(self, value, mod=None, /)
     |      Return pow(self, value, mod).
     |  
     |  \_\_radd\_\_(self, value, /)
     |      Return value+self.
     |  
     |  \_\_rdivmod\_\_(self, value, /)
     |      Return divmod(value, self).
     |  
     |  \_\_repr\_\_(self, /)
     |      Return repr(self).
     |  
     |  \_\_rfloordiv\_\_(self, value, /)
     |      Return value//self.
     |  
     |  \_\_rmod\_\_(self, value, /)
     |      Return value\%self.
     |  
     |  \_\_rmul\_\_(self, value, /)
     |      Return value*self.
     |  
     |  \_\_round\_\_(self, ndigits=None, /)
     |      Return the Integral closest to x, rounding half toward even.
     |      
     |      When an argument is passed, work like built-in round(x, ndigits).
     |  
     |  \_\_rpow\_\_(self, value, mod=None, /)
     |      Return pow(value, self, mod).
     |  
     |  \_\_rsub\_\_(self, value, /)
     |      Return value-self.
     |  
     |  \_\_rtruediv\_\_(self, value, /)
     |      Return value/self.
     |  
     |  \_\_str\_\_(self, /)
     |      Return str(self).
     |  
     |  \_\_sub\_\_(self, value, /)
     |      Return self-value.
     |  
     |  \_\_truediv\_\_(self, value, /)
     |      Return self/value.
     |  
     |  \_\_trunc\_\_(self, /)
     |      Return the Integral closest to x between 0 and x.
     |  
     |  as\_integer\_ratio(self, /)
     |      Return integer ratio.
     |      
     |      Return a pair of integers, whose ratio is exactly equal to the original float
     |      and with a positive denominator.
     |      
     |      Raise OverflowError on infinities and a ValueError on NaNs.
     |      
     |      >>> (10.0).as\_integer\_ratio()
     |      (10, 1)
     |      >>> (0.0).as\_integer\_ratio()
     |      (0, 1)
     |      >>> (-.25).as\_integer\_ratio()
     |      (-1, 4)
     |  
     |  conjugate(self, /)
     |      Return self, the complex conjugate of any float.
     |  
     |  hex(self, /)
     |      Return a hexadecimal representation of a floating-point number.
     |      
     |      >>> (-0.1).hex()
     |      '-0x1.999999999999ap-4'
     |      >>> 3.14159.hex()
     |      '0x1.921f9f01b866ep+1'
     |  
     |  is\_integer(self, /)
     |      Return True if the float is an integer.
     |  
     |  ----------------------------------------------------------------------
     |  Class methods defined here:
     |  
     |  \_\_getformat\_\_(typestr, /) from builtins.type
     |      You probably don't want to use this function.
     |      
     |        typestr
     |          Must be 'double' or 'float'.
     |      
     |      It exists mainly to be used in Python's test suite.
     |      
     |      This function returns whichever of 'unknown', 'IEEE, big-endian' or 'IEEE,
     |      little-endian' best describes the format of floating point numbers used by the
     |      C type named by typestr.
     |  
     |  \_\_set\_format\_\_(typestr, fmt, /) from builtins.type
     |      You probably don't want to use this function.
     |      
     |        typestr
     |          Must be 'double' or 'float'.
     |        fmt
     |          Must be one of 'unknown', 'IEEE, big-endian' or 'IEEE, little-endian',
     |          and in addition can only be one of the latter two if it appears to
     |          match the underlying C reality.
     |      
     |      It exists mainly to be used in Python's test suite.
     |      
     |      Override the automatic determination of C-level floating point type.
     |      This affects how floats are converted to and from binary strings.
     |  
     |  fromhex(string, /) from builtins.type
     |      Create a floating-point number from a hexadecimal string.
     |      
     |      >>> float.fromhex('0x1.ffffp10')
     |      2047.984375
     |      >>> float.fromhex('-0x1p-1074')
     |      -5e-324
     |  
     |  ----------------------------------------------------------------------
     |  Static methods defined here:
     |  
     |  \_\_new\_\_(*args, **kwargs) from builtins.type
     |      Create and return a new object.  See help(type) for accurate signature.
     |  
     |  ----------------------------------------------------------------------
     |  Data descriptors defined here:
     |  
     |  imag
     |      the imaginary part of a complex number
     |  
     |  real
     |      the real part of a complex number


        

    {\color{incolor}In [{\color{incolor}42}]:} \PY{c+c1}{\PYZsh{} Boolean}
             \PY{n}{a} \PY{o}{=} \PY{k+kc}{True}
             \PY{n+nb}{print}\PY{p}{(}\PY{n+nb}{type}\PY{p}{(}\PY{n}{a}\PY{p}{)}\PY{p}{)}

    <class 'bool'>

        

**Python Strings**

    1) string is sequence of unicode characters
    2) multi line string can be denoted using triple quotes - ''' or """ or \
    3) indexing starts from 0

    {\color{incolor}In [{\color{incolor}53}]:} \PY{n}{a} \PY{o}{=} \PY{l+s+s2}{\PYZdq{}}\PY{l+s+s2}{thisis deepa learning ai}\PY{l+s+s2}{\PYZdq{}}
             \PY{n+nb}{print}\PY{p}{(}\PY{n+nb}{len}\PY{p}{(}\PY{n}{a}\PY{p}{)}\PY{p}{)}
             \PY{n+nb}{print}\PY{p}{(}\PY{n}{a}\PY{p}{[}\PY{l+m+mi}{1}\PY{p}{:}\PY{p}{]}\PY{p}{)}
             \PY{n+nb}{print}\PY{p}{(}\PY{n}{a}\PY{p}{[}\PY{o}{\PYZhy{}}\PY{l+m+mi}{1}\PY{p}{]}\PY{p}{)}
             \PY{n+nb}{print}\PY{p}{(}\PY{n}{a}\PY{p}{[}\PY{p}{:}\PY{l+m+mi}{5}\PY{p}{]}\PY{p}{)} \PY{c+c1}{\PYZsh{} 0 to 4}
             \PY{n+nb}{print}\PY{p}{(}\PY{n}{a}\PY{p}{[}\PY{l+m+mi}{5}\PY{p}{:} \PY{o}{\PYZhy{}}\PY{l+m+mi}{1}\PY{p}{]}\PY{p}{)} \PY{c+c1}{\PYZsh{} before \PYZhy{}1}
             \PY{n+nb}{print}\PY{p}{(}\PY{n}{a}\PY{p}{[}\PY{n+nb}{len}\PY{p}{(}\PY{n}{a}\PY{p}{)} \PY{o}{\PYZhy{}} \PY{l+m+mi}{1}\PY{p}{]}\PY{p}{)}
             \PY{n+nb}{print}\PY{p}{(}\PY{n}{a}\PY{p}{[}\PY{o}{\PYZhy{}}\PY{l+m+mi}{25}\PY{p}{]}\PY{p}{)}

    24
    hisis deepa learning ai
    i
    thisi
    s deepa learning a
    i

        


            ---------------------------------------------------------------------------

            IndexError                                Traceback (most recent call last)

            <ipython-input-53-724f54baf981> in <module>()
              6 print(a[5: -1]) \# before -1
              7 print(a[len(a) - 1])
        ----> 8 print(a[-25])
        

            IndexError: string index out of range

        

**Python Lists**

    1) Order sequence of items
    2) objects can be multiple data types
    3) index starts from 0
    4) mutable

    {\color{incolor}In [{\color{incolor}54}]:} \PY{n}{a} \PY{o}{=} \PY{p}{[}\PY{l+m+mi}{10}\PY{p}{,} \PY{l+m+mf}{2.5}\PY{p}{,} \PY{l+s+s2}{\PYZdq{}}\PY{l+s+s2}{Deepa}\PY{l+s+s2}{\PYZdq{}}\PY{p}{]}
             \PY{n+nb}{print}\PY{p}{(}\PY{n}{a}\PY{p}{[}\PY{l+m+mi}{1}\PY{p}{]}\PY{p}{)}
             \PY{n+nb}{print}\PY{p}{(}\PY{n+nb}{type}\PY{p}{(}\PY{n}{a}\PY{p}{)}\PY{p}{)}

    2.5
    <class 'list'>

        

**Python Tuple**

    1) ordered sequnce of items
    2) objects can be multiple data types
    3) index starts from 0
    4) immutable 

    {\color{incolor}In [{\color{incolor}58}]:} \PY{n}{a} \PY{o}{=} \PY{p}{(}\PY{l+m+mi}{1}\PY{p}{,} \PY{l+m+mi}{1}\PY{p}{,}\PY{l+m+mi}{234}\PY{p}{,} \PY{l+m+mf}{346.7}\PY{p}{,} \PY{l+s+s2}{\PYZdq{}}\PY{l+s+s2}{asf}\PY{l+s+s2}{\PYZdq{}}\PY{p}{,} \PY{l+m+mi}{1} \PY{o}{+} \PY{l+m+mi}{2}\PY{n}{j}\PY{p}{)}
             \PY{n}{a}\PY{p}{[}\PY{l+m+mi}{4}\PY{p}{]}
             \PY{n}{a}\PY{p}{[}\PY{l+m+mi}{4}\PY{p}{]} \PY{o}{=} \PY{l+m+mi}{12}


            ---------------------------------------------------------------------------

            TypeError                                 Traceback (most recent call last)

            <ipython-input-58-288ddc83e195> in <module>()
              1 a = (1, 1,234, 346.7, "asf", 1 + 2j)
              2 a[4]
        ----> 3 a[4] = 12
        

            TypeError: 'tuple' object does not support item assignment

        

**Python Set**

    1) no indexing
    2) unordered collection
    3) unique items
    4) data structure
    5) multiple data types can be stored

    {\color{incolor}In [{\color{incolor}60}]:} \PY{n}{a} \PY{o}{=} \PY{p}{\PYZob{}}\PY{l+m+mi}{10}\PY{p}{,} \PY{l+s+s2}{\PYZdq{}}\PY{l+s+s2}{hello}\PY{l+s+s2}{\PYZdq{}}\PY{p}{\PYZcb{}}
             \PY{n+nb}{print}\PY{p}{(}\PY{n}{a}\PY{p}{)}

    \{'hello', 10\}

        

    {\color{incolor}In [{\color{incolor}61}]:} \PY{n}{a}\PY{p}{[}\PY{l+m+mi}{1}\PY{p}{]}


            ---------------------------------------------------------------------------

            TypeError                                 Traceback (most recent call last)

            <ipython-input-61-8bc71255a22e> in <module>()
        ----> 1 a[1]
        

            TypeError: 'set' object does not support indexing

        

**Python Dictionary**
