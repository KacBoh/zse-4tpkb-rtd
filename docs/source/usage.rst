Usage
=====

Nagłówek 1
==========

Nagłówek 2
----------

Nagłówek 3
~~~~~~~~~~

Nagłówke 4
^^^^^^^^^^

Akapit tekstowy

.. note:: akapit informacyjny note
.. tip:: akapit informacyjny tip

`kod linniowy`

<pre>kod
blokowy
</pre>

odnośnik wewnętrzny
:ref:`api

`Odnośnik zewnętrzny <https://edu.gplweb.pl/>`_

lista numerowana:
1. element1
2. element2

.. _installation:

Installation
------------

To use Lumache, first install it using pip:

.. code-block:: console

   (.venv) $ pip install lumache

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

