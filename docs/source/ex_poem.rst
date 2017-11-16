Week 4 - Poem Generation and Evaluation
=======================================

.. note::
    16.11.17 The assignments are not yet in their final form.

Introduction
------------

In the previous weeks, you have implemented several different methods for
generating creative text output. Your main task this week is to combine
these methods to build a system that generates poems.

Exercises
---------

#. **RETURN** *(Code)* Combine made-up fact generation (week 3.) and metaphor
   generation (week 2.) to produce a pair of poem lines.

   That is, on both lines of the poem you use at least one of the above mentioned
   methods. The rest of the lines you can produce, e.g. with your Markov model.

   The meter, rhyming, etc., are yours to design. The only requirement is that
   the two lines should be *connected* in some way. The connection can be, e.g.
   ensuring that a same word is used on both lines, they match semantically or
   in their sentiment, or something else.

   Concentrate on a simple implementation which produces varying output! You can
   also develop the made-up fact generation and metaphor generation further to
   achieve more varying poem lines.

   **In your code, clearly state what the code is supposed to do by commenting it.**

#. **RETURN** *(Code)* Combine two poem line pairs (from the above exercise) to
   create a four line poem. Again, you can design them any way you like, but
   the result should (hopefully) be "poem like", and there should be some
   connection between the pairs of lines.

   **In your code, clearly state what the code is supposed to do by commenting it.**

#. **RETURN** *(Code)* Poem evaluation. Design and implement a function
   ``evaluate(poem)``, which takes as input a single four line poem and outputs
   an evaluation for it.

   The function can measure any features from the poem you see as important.
   Again, concentrate on simple implementations which are maximally robust and
   give varying evaluations.

   **In your code, clearly state what the code is supposed to do by commenting it.**

#. **RETURN** *(Text Output)* Create poems in a loop and use your ``evaluate``
   function as a filter to throw away poems evaluated poor enough. Collect some
   5-10 poems which your code observes good enough and add them as your answer.
   Briefly, analyse your collected poems and their relation to evaluation and
   poem generation methods.

#. **RETURN** *(Text)* Some question about the article, hopefully in relation to
   the above questions.




