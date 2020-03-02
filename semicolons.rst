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