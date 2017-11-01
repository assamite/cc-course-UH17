Week 2 - Metaphor generation
============================

TODO: Khalid, add introductory text

Exercises
---------

#. **RETURN** *(Code)* Return to your code from last week's exercises, where you trained a Markov model
   on the text of *Alice's Adventures in Wonderland*.

   Alter your function ``markov_chain`` to accept an optional parameter ``order`` which
   specifies the order of the Markov chain to be created.

   That is, with ``order=2`` a state contains two successive tokens from the same sentence.

#. **RETURN** *(Code)* Create a new version of your function ``generate``,
   ``generate2(probs1, probs2, length=10, start=None)``. ``probs1`` and ``probs2`` are now expected to be the
   state transition distributions for an order-1 and an order-2 Markov model, respectively.

   This function should generate from the Markov model as before, except that, if it encounters a context
   of two words that does not exist in the order-2 model's distribution, it uses the order-1 model instead,
   treating just the single latest word as context.

   This is a form of a commonly used technique when working with Markov models, known as *backoff*.


TODO: Khalid's exercises to be added
