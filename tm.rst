=======================
A talk for ToastMasters
=======================

Level 1 Visionary Communication: Researching and Presenting

On the semicolon, its history and use in programming

Tuesday 12th January 2021

Introduction
============

* A little bit of history
* A little bit on usage
* The problems of typing
* The use in programming, which is my main interest

History
=======

Punctuation as we know it became standardised with the rise of printing in the
14th and 15 centuries.

The first printed semicolon was introduced in 1494 / the fifteenth century
by Aldus Manutius the Elder, who established its use to allow a rapid
change of direction when connecting independent statements.

Ben Jonson (born 1572, so 16th century) was the first English writer to use
it systematicaly.

English usage
=============

To join two complete thoughts that could stand alone as complete sentences.

Or, more formally, to link two closely related "independent clauses" in a
sentence; two clauses that are balanced, opposed, or contradictory.

For instance:

* She calls it the bathroom; I call it the loo.
* This is a Remington typewriter; all the keys are intact.

Also, separating elements of a list which themselves have
internal punctuation - in other words, because commas don't work.

(I've seen an argument that this is more common in US English)

In passing, it and the colon are probably the hardest punctuation to "hear".

I'd argue that the semicolon is the English punctuation you can most afford to
ignore. If that helps.

Early typewriters
=================

The QWERTY typewriter layout was invented in the early 1870s. It went through
several variants, most of which omitted several characters we would expect to
be there, particularly ``0``, ``1``, ``!`` and ``;``

Typists would use ``O`` and ``I`` for ``0`` and ``1``, and combine
``.`` and ``''`` for exclamation mark, and ``:`` and ``,`` for semicolon.

  Or: O for zero; I for 1; *full stop and quote* for exclamation mark; *comma
  and colon* for semicolon

In 1873 Remington bought the rights to the QWERTY typewriter, and added the
semicolon in (but still left out 1 and 0).

Programming
===========

Two main uses, both of which can be seen as a "pun" on joining
complete but separate related thoughts.

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

Lisp, since relatively early in its history (MacLISP in 19749 seems to be the
origin)

For some reason, I find the use as a comment character rather reassuring,
expecially in lisp.

Semicolon programming language
------------------------------

As a bonus, an "esoteric" (or joke) programmng language, Semicolon,
which uses only semicolons, reversed semicolons, spaces and newlines.

Finale
------

I think the semicolon has always been a bit of an oddity, and its use
indicates something about the writer.

Every so often, people mourn that its use is being forgotten in English
writing, or that no-one remembers *how* to use it any more.

But I don't actually see any real evidence of its disappearance - I still see
it being used in all sorts of fiction, for instance.

And it's clear the semicolon isn't going away in programming languages, where
people seem to be continually looking for subtle changes in its usage.

------------------

In a tweet in Feburary 2020 David MacIver asked:

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
