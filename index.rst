+--------------------------------+-----------------------------------+
| Paragraphs are flush-left,     | Literal block, preceded by "::":: |
| separated by blank lines.      |                                   |
|                                |     Indented                      |
|     Block quotes are indented. |                                   |
+--------------------------------+ or::                              |
| >>> print 'Doctest block'      |                                   |
| >>> print 'Doctest block'      |                                   |
| >>> print 'Doctest block'      |                                   |
| >>> print 'Doctest block'      |                                   |
| >>> print 'Doctest block'      |                                   |
| >>> print 'Doctest block'      |                                   |
| >>> print 'Doctest block'      |                                   |
| >>> print 'Doctest block'      |                                   |
| >>> print 'Doctest block'      |                                   |
| Doctest block                  | > Quoted                          |
+--------------------------------+-----------------------------------+
| | Line blocks preserve line breaks & indents. [new in 0.3.6]       |
| |     Useful for addresses, verse, and adornment-free lists; long  |
|       lines can be wrapped with continuation lines.                |
+--------------------------------------------------------------------+

Block Quotes
------------

Block quotes consist of indented body elements:

    My theory by A. Elk.  Brackets Miss, brackets.  This theory goes
    as follows and begins now.  All brontosauruses are thin at one
    end, much much thicker in the middle and then thin again at the
    far end.  That is my theory, it is mine, and belongs to me and I
    own it, and what it is too.

    -- Anne Elk (Miss)




Tables
------

Here's a grid table followed by a simple table:

+------------------------+------------+----------+----------+
| Header row, column 1   | Header 2   | Header 3 | Header 4 |
| (header rows optional) |            |          |          |
+========================+============+==========+==========+
| body row 1, column 1   | column 2   | column 3 | column 4 |
+------------------------+------------+----------+----------+
| body row 2             | Cells may span columns.          |
+------------------------+------------+---------------------+
| body row 3             | Cells may  | - Table cells       |
+------------------------+ span rows. | - contain           |
| body row 4             |            | - body elements.    |
+------------------------+------------+----------+----------+
| body row 5             | Cells may also be     |          |
|                        | empty: ``-->``        |          |
+------------------------+-----------------------+----------+



Results in:

  .. code-block:: python

      >>>Whitespace, newlines, blank lines, and all kinds of markup
      >>>(like *this* or \this) is preserved by literal blocks.
      >>>Lookie here, I've dropped an indentation level
      >>>print(but not far enough)
      
      
    
Stack
=====

Quick Start Guide
-----------------

.. code-block:: python


    # import the required data structure
    >>> from pythorn.data_structures.stack import Stack

    # creating a stack
    >>> a = Stack()

    # push elements
    >>> a.push(5)
    >>> a.push(20)
    >>> a.push(13)

    # displaying full stack
    >>> a.display()
    [5, 20, 13]

    # top element
    >>> a.tos()
    13

    # poping the element
    >>> a.pop()
    13
    >>> a.isEmpty()
    False



Stack Programs
--------------

.. automodule:: pythorn.data_structures.stack

    Stack
    -----

    .. autoclass:: Stack
       :members:


    Infix To Postfix
    ----------------

    Example :
        .. code-block:: python

            # importing Stack and Infix_Postfix
            >>> from pythorn.data_structures.stack import Stack 
            >>> from pythorn.data_structures.stack import Infix_Postfix

            # creating a stack
            >>> my_stack = Stack()

            # My Expression
            >>> my_exp = "a+c-*/dsefj-+//jk"

            # passing stack and expression to the Infix_Postfix class
            >>> infixpostfix = Infix_Postfix(my_exp,my_stack)
            >>> infixpostfix.infixToPostfix()
            'a c + * d s e f j / - - / j k / +'



    .. autoclass:: Infix_Postfix
       :members:


    Integer To Binary
    -----------------

    Example :
        .. code-block:: python

            # importing Stack and Integer_Binary
            >>> from pythorn.data_structures.stack import Stack 
            >>> from pythorn.data_structures.stack import Integer_Binary

            # creating a stack
            >>> my_stack = Stack()

            # My Number
            >>> my_num = 45

            # passing my_stack and my_num to the Integer_Binary class
            >>> integerbinary = Integer_Binary(my_num,my_stack)
            >>> integerbinary.IntegerBinary()
            '101101'
            

    .. autoclass:: Integer_Binary
       :members:




    











