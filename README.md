# explain - explanation pending.

A game of exploring space(s).  Language spaces. It is a game of 3 words and 3 bits (2x1.5).  You can swap the bits in E and I, which can take the normal values of 0 and 1, but also the values of / and 1/0.  The mystery continues in that you have to find paths, with words, that verify IN ALL CASES (IAC), but, it's up to you to verify that, probabilisically, your answer is correct.  That's because your only input is a RANDOM VALUE (RV), or a bit that can either be 1 or 0.  This is through the use of the first word, 'tri', as follows:

```sh
    $ explain 1/0 / tri
```

This is the first word.  tri will take the contents of the E LOCATION and give it a random value of 1 or 0 if it's contents were intiall /, aka 1/0.  The intial contents are always / at the start of *every run*, so you always get a fresh start with every sentence.

From there you will prove sentances.  The words will follow and you will find the resulting values.  I mean, there's only 2 bits, it can't be that hard to figure them out, right?   It's up to you to see how long a string of words you can make, and also, how little debugging output you can have and if you get a 'pass' at the end.  That's the competition.  The longest amount of words with the least output.  Hopefully, the sentences might even do something useful (someday).

This is really a game about metaprogramming.  You will not, for long, want to program in the base #Logica itself.  You will want to design a META PROGRAMMING (MP) system, one whic will GENERATE YOUR CODE (GYC) for you. This because, with so few words (although it's Turing Complete[2]), writing it by itself, I think, will get boring quite quickly.

I have defined the word 'meta', a higher level word, one which feeds data into 'explain':

```
    meta is the next word after tri, swap and not
    
    SYNTAX: meta <word> <explanation ...>
    
      meta is 'meta'.
    
      <word> is a string of characters surrounded by white space.
      
      <explaination> is a string of words.
      
    SUMMARY:
      
      meta will define a word as an explanation.
      
      when meta encounters a word with an explanation, it replaces that word with the explanation.
      
      that's it.
      
   BUGS:
   
      I hope not.
      
  AUTHOR:
  
      TMD Inc.
```

See 'expect', in the top level of the repsitory.  Check it's history for more explanation.

This program runs best on macOS or Solaris[1]. 

--
BusFactor1 Inc.
Burton Samograd
root@busfactor1.ca
http://busfactor1.ca/
2017

[1] Real UNIX based operating systems. The ones with Korn Shell by deafult.
[2] Citation Needed.

References
==========

MetaMaths! - Gregory Chaitin
Exploring Randomness - Gregory Chaitin
The Limits of Mathematics - Gregory Chaitin
The Unknowable - Gregory Chaitin
Proving Darwin - Gregory Chaitin
Principia Mathematica - Russel and Whitehead
Algorithms - various
