=======================
Fashions in semi-colons
=======================

In a tweet in Feburary 2020 (thread was at
https://twitter.com/DRMacIver/status/1228346166150123521)
David MacIver asked:

  Scenario: You are given one calendar year to take a sabbatical and write a
  book. You are paid a sufficient salary to focus exclusively on it, and
  provided an editor, etc. to handle publishing, you just need to do the
  actual writing. What do you write?

And I responded:

  Given a year and a good editor, then I'd want to write an overview of the
  programming languages that seem to me to be interesting over the last 50
  years or so. There were a couple of these in the 80s/90s, which I enjoyed a
  lot.

  It would need to be very personal - there's no way to do a "proper" history
  in reasonable space, but I think there's room for "these are the things that
  happened (in programming languages) that seem interesting to me" and also
  how they relate (or don't)

  (Of course, I think a chapter on the changing fashions and meanings of
  semi-colons would be interesting, so perhaps you don't really want me to do
  this)

  Drat - now I want to write that. Drat.

I'm fairly convinced no-one would want to read this or listen to it...

* Where did their use come from? Who used them first
* Languages where a semicolon is a comment character (lisp, assembly) [nb:
  neither of those needs a traditional terminator character, but for entirely
  different reasons)
* Separator or terminator (C or Pascal)
* Required or optional
* If optional, why ever need them
* (how to tell if a line continues - strategies in BCPL, Ruby, who else?)
* If required, why
* What does the compiler do if a user misses one?
* Programming languages that use other characters (erlang, prolog)
* Rust and the meaning when a semicolon *isn't* there



Things:

- the use of the semicolon in the english language
- early languages didn't need to mark end of statement/expression: assembly,
  Fortran, Lisp
- comments in lisp and assembly
- Introduction of semicolons - continuation or separation
- Complementary concept - continuation characters (this statement/expression
  continues on the next virtual line)
  
  - BCPL continuation of statement/expression - check BCPL syntax?
  - backslash to escape newline - what about white space after it
  - a character at the start of the *next* line to indicate continuation
    (?BCPL also?)
  - the time GNU make (I think it was) changed its convention about that

- Other languages using, e.g., ``.`` - Erlang and I think Prolog?
- Optional semicolons - Python, Ruby - use to allow multiple statements or
  expressions on one line
- Optional semicolons - JavaScript - if omitted, it will try to guess
- Compiler strategies if they're missing
- Rust - distinction between line ending with semicolon and line not

----------------------------

Useful links
============

* https://www.newyorker.com/books/page-turner/semicolons-so-tricky

  Quoting a small book called "Punctuation...?": "A semicolon links two
  balanced statements; a colon explains or unpacks the statement or
  information before it."

* https://www.userdesignillustrationandtypesetting.com/books/punctuation/index.html
  - the homepage for that same book

* https://en.wikipedia.org/wiki/Semicolon

* https://www.wglt.org/post/history-semicolon-and-how-use-it - The History Of
  The Semicolon (And ... How To Use It) - contains a reference to the book
  "Semicolon: The past, present and future of a misunderstood mark" by Cecelia
  Watson

* https://smile.amazon.co.uk/Semicolon-misunderstood-punctuation-improve-writing-ebook/dp/B07MLPMS3N
  - Semicolon: How a misunderstood punctuation mark can improve your writing,
  enrich your reading and even change your life - presumably the same book
  under a slightly different name?

* https://examples.yourdictionary.com/examples-of-colons-and-semicolons-in-sentences.html
  - some nice examples

* https://www.ole.bris.ac.uk/bbcswebdav/courses/Study_Skills/grammar-and-punctuation/index.html#/id/5eaff0ce88d7eb04c5efb446
  - English usage of semicolon in lists, as well as the closely-related
  independent clases usage

* https://en.wikipedia.org/wiki/QWERTY#Combined_characters - using a colon and
  comma to produce a semicolon on early QWERTY typewriters

* https://medium.com/better-programming/a-brief-history-of-the-8efda9dde2b8 -
  A Brief History of the Semicolon in Programming (as a separator/terminator
  for statements)

* http://www.softwarepreservation.org/projects/LISP/MIT/Moon-MACLISP_Reference_Manual-Apr_08_1974.pdf
  - MacLISP manual showing use of semicolons for comments (page 3)

* https://www.reddit.com/r/lisp/comments/fqs19u/differences_between_lisp_15_and_common_lisp_part_1/
  - "The semicolon comment used in Common Lisp comes from Maclisp. Maclisp
  likely got it from PDP-10 assembly language, which let a semicolon and/or
  a line break terminate a statement; thus anything following a semicolon is
  ignored."

* https://pksunkara.com/semicolon/ - the "esoteric" programming language
  Semicolon, which uses only semicolons, reversed semicolons, spaces and
  newlines

* https://lucumr.pocoo.org/2012/10/18/such-a-little-thing/ - Armin Ronacher on
  semicolons in rust, and why they work as they do (and a discussion of Python
  and Ruby on the way)

----------------------------

=======================
A talk for ToastMasters
=======================

Level 1 Visionary Communication: Researching and Presenting

On the semicolon, its history and use in programming

Tuesday 12th January 2021

History
=======

Aldus Manutius the Elder introduced the first printed semicolon in 1494, and
established its use to separated words of opposed meaning and to allow a rapid
change if direction when connecting independent statements.

Ben Jonson (born 1572) was the first English writer to use it systematicaly.

English usage
=============

To link two closely related "independent clauses" in a sentence, when the
clauses are balanced, opposed, or contradictory. Or, in other words, to join
two complete thoughts that could stand alone as complete sentences.

For instance:

* She calls it the bathroom; I call it the loo.
* This is a Remington typewriter; all the keys are intact.

Also, separating elements of a list which themselves have
internal punctuation - in other words, because commas don't work.

(I've seen an argument that this is more common in US English)

When spoken, and particuarly in the first usage, my experience is to treat it
as a pause of length between a comma and a colon. If that helps...

Early typewriters
=================

The QWERTY typewriter layout was invented in the early 1870s. It went through
several variants, most of which omitted several characters we would expect to
be there, such as 0, 1 and the exclamation mark and semicolon.

Typists would use O and I for 0 and 1, and combine full stop and quote for
exclamation mark, and colon and comma for semicolon.

In 1873 Remington bought the rights, and added the semicolon in (but still
left out 1 and 0).

Programming
===========

3 types of use, two of which work as puns on its use in written English.

Statement delimitor
-------------------

5 usages (at least):

* Compulsory statement terminator - e.g., C

  (unhelpful if you forget one!)

* Optional statement terminator - e.g., Javascript

  (confusing - exactly when can it be omitted, and what happens if yoi get it wrong)

* Compulsory statement separator - e.g., Algol 60 and Pascal

  (confusing, hard to remember it's not a separator)

* Newline equivalent - e.g., Python

  (only used to make code fit on one line isntead of several)

* Rust - presence means throw the expression value away, absence means
  "return" it

(instead of using ``return``, which would presumably look odd for the branch
of an ``if`` expression. compiler presumably helps a lot with its type checking)

Note: languages such as erlang and prolog use ``period`` (full stop) instead
of semicolon.

Comment delimitor
-----------------

Assembly languages

Lisp, since relatively early in its history (MacLISP in 197491G)

Finale
------

Every so often, people mourn that the semicolon is being forgotten in English
writing, or that no-one remembers how to use it any more. I think it's always
been a bit of an oddity, and its use indicates something about the writer.

But I don't actually see any real evidence of its disappearance - I still see
it beign used in all sorts of fiction, for instance.

And it's clear the semicolon isn't going away in programming languages.
