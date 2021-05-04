=====================
Why I quite like Ruby
=====================

or: The path not taken (by Python)

or: Why I like Python, quite like Ruby, and might be learning Common lisp


-------


* OO, but not the same sort of OO
* Value or method - done entirely differently, but about as easy
* Lisp-1 versus Lisp-2
* Naming a value evaluates it (which may mean calling it)
* Python - callables. Ruby - messaging.
* Optional ``()`` for method calling
* Blocks ending with ``end``
* Passing a block to a method - fundamental control structure
* Nobody uses the ``for`` loop
* rbenv and bundle =~= pyenv and poetry/pipenv
* rspec - almost cucumber
* rspec - hamcrest style matchers, ease of mocking
* ``"#{<expression}"`` - compare with ``f`` strings

-------

In Python, "naming" a callable does not call it:

* Naming anything is just naming it
* ``a = b`` is distinguished from ``a = b()`` - the "call" operator (``()``)
  may cause ``b`` to respond with a different result, depending on if it has
  a ``__call__`` method.

In Ruby, ``b`` may well call ``b``.

-------

Lisp-1 versus Lisp-2

-------

rspec as "cucumber light"

Simple example

More complicated example with mockingbird

-------

Ruby wanting to be "easy to write" more than "easy to read" (but still
readable) - compare with Python

------

Zen of Python - compare ruby

------

rbenv and bundle (similar to pyenv and poetry/pipenv)

-------

Like Python, Ruby is solidly built on well-proven ideas from programming
history. Just not the same ideas.

------

Blocks end with ``end`` (regardless of how they start)

------

Python: "everything is an object", but multi-paradigm

Ruby: totally object oriented, "old school". Ends up being "upside down" to Python.

* All callables are methods, but it doesn't mean you *have* to declare a class

* Actually, sending messages to objects - so ``obj.send(:thing")``, which (for
  instance) allows one to override ``private``

* It's quite easy to define how to catch a message that has no corresponding
  method, and so do the appropriate thing with it.

* Python: assume an ``a.x`` is a value, but can add plumbing to make it be a
  method call.

* Ruby: ``a.x`` is always a setter/getter method call. *But* there's syntax to
  set that up with one line (double check what it is!)::

    attr_reader x

-------

``3.times``, ``1..5``, ``1...5``.times

There are ``for`` loops, but no-one uses them.

Relies on *blocks* - which relies on having block delimiters, i.e., ``begin``
and ``end``

``yield`` means "take the block we were passed (as an argumetnt) and execute
it as if it replaced this ``yield``"

Can pass the block as the last declared argument (``(..., &block)``) or can
pass it "outside" the argument list. In the latter case, there's a call to see
if the method was given a block argument or not.

-------

Ruby much more likely to add synonyms for things - much less interested in
"only one way". Instead, wants to give the predictable way (and thus easier
to write).

--------

Ruby - ``require`` is essentially ``from xxx import *`` and appears to be the
norm

--------

Don't forget Ruby has symbols - hard to understand how useful these are if
you've not used them.

---------

...
