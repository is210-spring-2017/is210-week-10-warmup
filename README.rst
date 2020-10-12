####################
IS 210 Assignment 8
####################
************
Warmup Tasks
************

:College: CUNY School of Professional Studies
:Course-Name: Software Application Programming I
:Course-Code: IS 210

Overview
========

The Python dict class is Python's core mapping-type. With it, data may be
stuctured and related with meaningful keys which opens a huge realm of program
capabilities.

Instructions
============

The following tasks will either have you interacting with existing files in
the assignment repository or creating new ones on the fly. Don't forget to add
your interpreter directive, utf-8 encoding, and a short docstring with any new
files that you create!

.. important::

    In these exercises, you may, on occasion, come across a task that requres
    you to research or use a function or method not directly covered by the
    course text. Since Python is such a large language it would be impossible
    for the author to have included descriptions of each and every available
    function which would largely duplicate the offical Python documentation.

    A *vital* skill to successful programming is being comfortable searching
    for and using official language documentation sources like the
    `Python String Documentation`_ page. Throughout our coursework we will be
    practicing both the use of the language in practice and the search skills
    necessary to become functional programmers.

Warmup Tasks
============


Task 01
-------


It is often very useful to iterate through a dictionary object separating the
iteration into key and value pairs. In this task you will need to use your new
knowledge of dictionary iteration using the ``iteritems()`` method.

Specifications
^^^^^^^^^^^^^^

#.  Use a new cell in your notebook

#.  Declare a variable named ``DATA`` as a dictionary object. Assign the  set
    of key/value pairs shown below.

#.  Create a function named ``iter_dict_funky_sum()`` that takes one
    dictionary argument.

    #.  Declare a running total integer variable.

    #.  Extract the key/value pairs from ``DATA`` simultaneously in a loop. Do
        this with just one ``for`` loop and no additional forms of looping.

    #.  Assign and append the product of the value minus the key to the running
        total variable.

    #.  Return the funky total.

Dictionary Data
^^^^^^^^^^^^

.. code:: python

    DATA = {
        2: 7493945,
        76: 4654320,
        3: 4091979,
        90: 1824881,
        82: 714422,
        45: 1137701,
        10: 374362,
        0: 326226,
        -15: 417203,
        -56: 333525,
        67: 323451,
        99: 321696,
        21: 336753,
        -100: 361237,
        55: 1209714,
        5150: 1771800,
        42: 4714011,
        888: 14817667,
        3500: 13760234,
        712: 10903322,
        7: 10443792,
        842: 11716264,
        18584: 10559923,
        666: 9275602,
        70: 11901200,
        153: 12074784,
        8: 4337229
    }

Expected Output
^^^^^^^^

.. code:: pycon

    >>> iter_dict_funky_sum(DATA)
    140166242



Submission
==========

Code should be submitted via Blackboard.

.. _Python String Documentation: https://docs.python.org/2/library/stdtypes.html
