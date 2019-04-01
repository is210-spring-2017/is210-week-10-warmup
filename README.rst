####################
IS 210 Assignment 10
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

There are a number of ways to access data from dictionaries. Here we'll
practice a few of the most common ones.

Specifications
^^^^^^^^^^^^^^

#.  Start off by opening ``data.py`` and just taking a look at the structure of
    the ``BANDS`` dictionary.

#.  Create a new notebook 

#.  import the ``data`` module.

#.  In one line, create a new constant named ``NIGEL`` and use dictionary keys
    to assign its value value from the ``'Nigel Tufnel'`` entry of the
    ``data.BANDS`` dictionary.

#.  Create a new constant named ``BANDS_NAMES`` and use a built-in dictionary
    function to fill it with a list of band-names from ``data.BANDS``.

Expected Output
^^^^^^^^

.. code:: pycon

    
    >>> NIGEL
    ['guitar', 'vocals', 'bass', 'violin', 'harmonica', 'clarinet',
     'keyboards', 'piano']
    >>> BAND_NAMES
    ['The Rolling Stones', 'Van Halen', 'Spinal Tap', 'Queen', 'The Beatles',
     'The Who', 'Fleetwood Mac']

Task 02
-------

There are a number of ways to add or remove keys to Python dictionaries. Here,
we'll cover the most common types.

Specifications
^^^^^^^^^^^^^^

#.  We will use the ``data`` module again (do this on a new cell in your notebook)

#.  copy ``data.BANDS`` into a new constant named
    ``CORRECTED``.

    .. tip::

        Keep in mind that the assignment operator (``=``), doesn't create a new
        dictionary, it just creates a new reference to it. There is a built-in
        dictionary function that creates a new copy of a dictionary.

#.  Using the assignment syntax (``[]``) add a new entry to ``CORRECTED``
    with a key value of ``Dylan`` and the following value:

    .. code:: python

        {'Bob Dylan': ['vocals', 'guitar', 'harmonica']}

#.  Remove the ``'David Lee Roth'`` entry from the ``'Van Halen'`` entry of
    ``CORRECTED`` with the ``del`` statement.

#.  Using the assignment syntax (``[]``), add a new entry to
    ``CORRECTED['Van Halen']`` with key ``'Sammy Hagar'`` and value
    ``['vocals']``.

Expected Output
^^^^^^^^

.. code:: pycon

    >>> CORRECTED['Van Halen'].keys()
    ['Eddie Van Halen', 'Sammy Hagar', 'Michael Anthony', 'Alex Van Halen']

Task 03
-------

The ``.update()`` method is a powerful tool for merging dictionary data as
you'll see below.

Specifications
^^^^^^^^^^^^^^

#.  Use a new cell in your notebook

#.  Create a new top-level band entry in ``data.BANDS``
    with the key, ``'Buckingham Nicks``. The key:values of ``Buckingham Nicks``
    are:

    .. code:: python

        'Lindsey Buckingham': ['guitar', 'vocals'],
        'Stevie Nicks': ['vocals', 'tambourine']

#.  Use a built-in dictionary function to merge 
    ``data.BANDS['Buckingham Nicks']`` into 
    ``data.BANDS['Fleewood Mac']`` so that there are now five keys in
    ``data.BANDS['Fleetwood Mac']``.

Task 04
-------

Changing dictionary values is nearly identical to assigning them.

Specifications
^^^^^^^^^^^^^^

#.  Use a new cell in your notebook

#.  Change the value of ``data.SUPERHEROES['Logan']['alias']`` to
    ``'Wolverine'`` without altering ``data.py`` and without creating a new
    dictionary or variable.


Task 05
-------

It is often very useful to iterate through a dictionary object separating the
iteration into key and value pairs. In this task you will need to use your new
knowledge of dictionary iteration using the ``iteritems()`` method.

Specifications
^^^^^^^^^^^^^^

#.  Use a new cell in your notebook

#.  Declare a variable named ``DATA`` as a dictionary object. Assign it a set
    of key/value pairs. This is example data for you to work with but you may
    create any dictionary of data provided it is at least 10 items long and
    both keys and values are integers.

#.  Create a function named ``iter_dict_funky_sum()`` that takes one
    dictionary argument.

    #.  Declare a running total integer variable.

    #.  Extract the key/value pairs from ``DATA`` simultaneously in a loop. Do
        this with just one ``for`` loop and no additional forms of looping.

    #.  Assign and append the product of the value minus the key to the running
        total variable.

    #.  Return the funky total.

Example Data
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
