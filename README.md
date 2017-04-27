
Install leinigen.

Setup clojure layer in spacemacs.


Moving from lisp/scheme to clojure :

https://www.youtube.com/watch?v=cPNkH-7PRTk


Start repl with lein repl


Why target JVM?
A good managed environment.
The intermediate languages are independent of source language.
Some ability to call/consume Java is critical

Why not OO?
Encourages mutable State
Polymorphism shoudn't be only on types.

What makes clojure a different lisp ?

1. more first class data structures.
2. Defined in terms of abstractions.
3. Functional/Immutable
4. Host embracing
5. Concurrency/Thread aware.

Its a lisp-1 (lexically scoped)

Symbols and vars are diffrent.
Java Null is clj nil.

Clojure has more first class datastructures with read/print support.
Clojure data structures are aslo strucuturally recursive.
Clojure like other dynamic languages has first class associative data
strucutures.

List of clojure data structures (Everything nests):
  1. Lists e.g. (1 2 3 4 5) , grow at front
  2. Vectors e.g. [1 2 3 4] , grow at end
  3. Maps - hashed and sorted e.g. {:a 1, :b 2, :c 3}
  4. Sets - hashed and sorted e.g #{fred ethel lucy}


Uniform 'add' - conj

Abstracting away the Cons cell - Seqs
Seq abstraction interface: first and rest
seq implemented for all Clojure collections,
all java collections, strings, regex matches, files


Maps and Sets are functions of their keys.
Indexed Vectors are function of index.



Lazy seq: 
first and rest are not produced until requested.

In clojure anything that can be lazily evaluated, is lazily evaluated.
