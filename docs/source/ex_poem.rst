Week 4 - Poem Generation and Evaluation
=======================================

.. note::
    16.11.17 The assignments are not yet in their final form.

Introduction
------------

In the previous weeks, you have implemented several different methods for
generating creative text output. Your main task this week is to combine
these methods to build a system that generates poems.

The exercises will give you a lot of freedom to design your own way of producing
poems. This might sound demanding to some, but this is a typical case in computational
creativity. There are no pre-given instructions on how to tackle the problem.
Therefore, you as a system's designer must reason on your choices and pick the
right tools.

*Have fun, and be creative while developing your poem system!*

Exercises
---------

#. **RETURN** *(Code)* Combine made-up fact generation (week 3.) and metaphor
   generation (week 2.) to produce two lines of a poem.

   That is, on both lines of the poem you use at least one of the above mentioned
   methods. The rest of the lines you can produce, e.g. with your Markov model.
   An example would be to:

        - start the first line with a made-up fact and produce the rest of the
          line with Markov model, and
        - end the second line with a metaphor, producing the start of the line
          with the Markov model (to be able to produce text from end to start, you
          have to train another Markov model from the reversed corpus).

   The meter, rhyming, etc., are yours to design. The only requirement is that
   the two lines should be *connected* in some way. The connection can be, e.g.
   ensuring that a same word is used on both lines, they match semantically or
   in their sentiment, or something else.

   Concentrate on a simple implementation which produces varying outputs! You can
   also develop the made-up fact generation and metaphor generation further to
   achieve more varying poem lines.

   **In your code, clearly state what the code is supposed to do by commenting it.**

   .. note::
        Use existing tools as much as you like. For example:

            - `a simple Python library for CMU's pronunciation dictionary <https://pypi.python.org/pypi/pronouncing>`_
            - `NLTK's various tools <http://www.nltk.org/book/>`_
            - `assorted web services done by the creative language group in UCD <http://afflatus.ucd.ie/article.do?action=list&categoryId=4>`_
            - etc.

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




