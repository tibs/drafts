====================================
Ruby: taking the paths Python didn't
====================================

Ruby is *not* inspired by Python, but Matz was definitely knowledgable about
it, and if Ruby does something differently, it is in full knowledge of this.

So Ruby is in many ways "the path not taken".

It's also a language one's not likely to learn if one already knows Python
(unless, as in my case, work needs one to).

* optional "call operators" (i.e., ``(`` and ``)``) leads to what look very
  like DSLs
* rspec
* Python has instance values which can be turned into function calls.
  Ruby instead makes it trivial to create getters and setters, and never
  exposes instance values. The *effect* is amazingly similar - except when it
  isn't (is that interesting?)


Blocks are cool but sort of boring.

mini-Ruby implementations not bothering to implement "for" loops is
interesting (one naturally uses ``.each`` and so on).
