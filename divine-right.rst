=================================================
So you think you might have Divine Right of Kings?
=================================================

NB: Intended to be exactly 5 minutes long, to be usable as a lightning talk or
as a toastmasters exercise.

An information pamphlet (or, an informational talk)

  Good day, gentles <bows>

  This is informational talk 379B, "So you think you might have Divine Right
  of Kings", as officially sanctioned by the Central Committees of the
  Communard Commiserate. Written versions may be obtained from your local
  Committee offices, and from your local Biblioteque.


ref: the wikipedia article on the Paris Commune (*very* peripherally)


The source code (more or less) for the game I wrote at PyCon UK 2019, in
Hannah's RenPy workshop:

  **start**

    "Welcome to 'So you have the Divine Right to be King', a helpful and
    instructive pamphlet for children from the socialist committee for our
    state."

    "Once upon a time, states were ruled by Kings (or, sometimes, Queens or
    Pharoahs or whatever)."

    "And this was OK because God had said that the ruler was King (or Queen
    or whatever), and that people should do what they said."

    "Sometimes the King (or Queen or whatever - we shan't keep saying that,
    but remember that we don't only mean actual Kings) was happy being King."

    "Sometimes the King was not happy being King."

    "Sometimes the people were happy with their King."

    "Sometimes the people were not happy with their King."

    "Today we don't have Kings (or Queens or Pharoahs) to tell us what to do.
    Instead we are a socialist state, and all work together to work out what we should do."

    "But sometimes people still find they've got the Divine Right to be
    King, and if that's you, this pamphlet should help you decide what to do."

    "So, do you have the Divine Right to be King?"

  **menu**

    "yes": jump divine_right

    "no": jump normal_person

  label **divine_right**

    "Let's see if we can help you!"

    "Do you like running things?"

  **menu**

    "yes": jump like_running_things

    "no": jump running_boring

  label **like_running_things**

    "You may have a future on one of the state committees, helping other
    people run things! If you're good at it, you may even get to be chair of a
    committee. With Divine Right of Kings, this can mean you have a fulfilling
    and helpful life as a useful member of the state! Get inolved with your
    local committee's junior branch and help us make this a better state!"

    jump end

  label **running_boring**

    "Because you've got Divine Right to be King, God will keep trying to
    push you to run things. But we can help!"

    "Do you like explaining things?"

  **menu**

    "yes": jump explaining

    "no": jump not_explaining

  label **explaining**

    "If you like explaining things, then being a teacher or a propagandist
    might be for you. Both are useful to the state, but look like running
    things to God, so will keep Them happy. Talk to your own teacher, or your
    local committee liaison to find out which choice suits you best."

    jump end

  label **not_explaining**

    "Life is more difficult if you have Divine Right of Kings but don't want
    to run things or tell people what to do."

    "Luckily, we know that the state also needs disruptive elements, and
    trying to distrupt the state (and replace it with something that might be
    better) is still the sort of thing God will be happy with. Contact your
    local state sponsored resistance movement to find out how you can help
    subvert the state, and keep it healthy by stopping it being complacent."

    jump end

  label **normal_person**

    "You're very lucky - having the Divine Right to be King is not much fun!"

    jump end

  label **end**

    # This ends the game.

    "Thank you for reading this, which is is one of the series of pamphlets
    called 'Statecraft with fun' - see your local library for the others!\n"
