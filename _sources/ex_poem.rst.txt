Week 4 - Poem Generation and Evaluation
=======================================

.. note::
    20.11.17 17:01 The assignments are in their final form.

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

#. **RETURN** *(Code)* Design an implement a function ``couplet(*args, **kwargs)``,
   where you combine made-up fact generation (week 3.) and figurative language generation (week 2.)
   to produce two lines of a poem.

   To produce the lines, you use at least once the made-up fact generation and once
   figurative language generation. The rest of the lines you can produce, e.g. with your Markov model.
   An example would be to:

        - start the first line with a made-up fact and produce the rest of the
          line with Markov model, and
        - end the second line with an analogy and producing the start of the line
          with the Markov model (to be able to produce text from end to start, you
          have to train another Markov model from the reversed corpus).

   The possible ``*args`` and ``**kwargs`` given to the function should be clearly
   described in the function's doc string.

   The meter, rhyming, etc., are yours to design. The only requirement is that
   the two lines should be *connected* in some way. The connection can be, e.g.
   ensuring that a same word is used on both lines, they match semantically or
   in their sentiment, or something else.

   Concentrate on a simple implementation which produces varying outputs! You can
   also develop the made-up fact generation and figurative language generation further to
   achieve more varying poem lines.

   **Submit runnable code (call the ``couplet`` function with appropriate arguments in your code so that it is runnable from the command line). Also, clearly state what the code is supposed to do by commenting it.**

   .. note::
        Use existing tools as much as you like. For example:

            - `a simple Python library for CMU's pronunciation dictionary <https://pypi.python.org/pypi/pronouncing>`_
            - `NLTK's various tools <http://www.nltk.org/book/>`_
            - `assorted web services done by the creative language group in UCD <http://afflatus.ucd.ie/article.do?action=list&categoryId=4>`_
            - etc.

#. **RETURN** *(Code)* Design and implement a function ``generate_poem(*args, **kwargs)``,
   where you combine two couplets (from the above exercise) to
   create a four line poem. Again, you can design the function any way you like, but
   the result should (hopefully) be "poem like", and there should be some
   connection between the pairs of lines. Hopefully, you can introduce some
   interesting twists between the couplets.

   The possible ``*args`` and ``**kwargs`` given to the function should be clearly
   described in the function's doc string.

   **Submit runnable code (call the ``generate_poem`` function with appropriate arguments in your code so that it is runnable from the command line). Also, clearly state what the code is supposed to do by commenting it.**

#. **RETURN** *(Code)* Poem evaluation. Design and implement a function
   ``evaluate(poem, *args, **kwargs)``, which takes as input a single four line poem and outputs
   an evaluation for it.

   The possible ``*args`` and ``**kwargs`` given to the function should be clearly
   described in the function's doc string.

   The function can measure any features from the poem you see as important.
   Again, concentrate on simple implementations which are maximally robust and
   give varying evaluations.

   Examples of evaluation (you don't have to use as many criteria, and we encourage you to implement your own ideas):

        - Is the rhyming in the whole poem consistent?
        - Does the poem match to a certain meter, e.g. a meter in Kalevala or a limerick?
        - Is the poem semantically sound?
        - Is the word 'cat' in the poem?
        - Does the poem talk about animals in general?
        - Does the poem contain synonyms?
        - Is the poem likely to evoke an emotion? (see `wordnet-affect <http://wndomains.fbk.eu/wnaffect.html>`_)
        - How balanced are the consonants and vowels in the poem?
        - Is the poem grammatically correct?

   **Submit runnable code (call the ``evaluate`` function with appropriate arguments in your code so that it is runnable from the command line). Also, clearly state what the code is supposed to do by commenting it.**

#. **RETURN** *(Text Output)* Create poems in a loop and use your ``evaluate``
   function as a filter to throw away poems evaluated poor enough. Collect some
   5-10 poems which your code observes good enough and add them as your answer.
   Briefly, analyse your collected poems and their relation to your intent with
   the generation. Reflect your analysis on your implementations of the poem
   evaluation and generation methods.

#. **RETURN** *(Text)* (200 words) Imagine your poem producing system as a part of a larger
   agent society. How could it take advantage of the domain or the field as
   described by Csikszentmihalyi's systems view of creativity (see, `Saunders and Gero: Artificial creativity: A synthetic approach to the study of creative behaviour <http://cs.gmu.edu/~jgero/publications/2001/SaundersGeroHI01.pdf>`_)?
   What kind of emergent behavior could the system gain from these aspects?
   What kind of emergence could the system induce in the whole society?




